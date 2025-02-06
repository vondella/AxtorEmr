# Axtor EMR
``` power shell
$version="1.0.6"
$owner="vondella"
dotnet pack src\Common\  --Configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/AxtorEm  -o ..\packages
