[![Board Status](https://dev.azure.com/yjwon0463/ec55e749-853d-4260-bc36-d7312fc53cdc/cf355d26-6683-4974-a048-bfb33e4ce79d/_apis/work/boardbadge/6e73c944-bea4-42dc-9f7b-1f87fd9df616)](https://dev.azure.com/yjwon0463/ec55e749-853d-4260-bc36-d7312fc53cdc/_boards/board/t/cf355d26-6683-4974-a048-bfb33e4ce79d/Microsoft.RequirementCategory)
# Azure DevOps HOL

This is the source code for Azure DevOps HOL by taking an example of a documentation project.

The documentation can be hosted on any HTML repositories including your GitHub Pages, from the *gh-pages* branch.

## Running locally

1. Run `dotnet run -p generator/src/generator.csproj -- . "http://localhost:8000/" _site` to build the HTML files.
2. Run `./copy-assets.bash _site` to copy assets into the target directory.
3. Run `python3 -m http.server 8000 --directory _site/` (or whatever your favorite static http server is) to serve the website at port 8000.
4. Open `http://localhost/:8000` in your web browser to view the result.
