# Axtor EMR
``` power shell
$version="1.0.6"
$owner="vondella"
dotnet pack src\Common\  --Configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/AxtorEm  -o ..\packages

Add Github Package source
$owner="vondella"
$gh_pat=['gh_access token']
dotnet nuget add source --username username --password $gh_pat --store-paasword-in-clear-text --name github "https://nuget.pkg.github.com/$owner/index.json"
