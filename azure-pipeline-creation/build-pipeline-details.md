# Build Pipeline Details

This file outlines the steps configured in the Azure DevOps Build Pipeline.

## 🔧 Pipeline Tasks Used

1. **NuGet Tool Installer**
   - Installs the required NuGet version for the build.

2. **NuGet Restore**
   - Restores all required packages for the .NET application.

3. **MSBuild**
   - Builds the application and generates the deployable output (.dll files).
   - Uses custom MSBuild arguments for publishing the web app.

4. **Publish Artifacts**
   - Publishes the output to Azure DevOps Artifacts so it can be used in the release pipeline.

## 🔄 Notes

- **Copy Files task** is disabled since we are directly publishing using MSBuild to the `$(Build.ArtifactStagingDirectory)` folder.
- Output files mainly include `.dll` and other necessary deployment files.
- Build pipeline is linked to the Azure Repos repository containing the application code.

