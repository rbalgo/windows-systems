## Usage Details

$moduleName = 'RBUtils'
$plaster = @{
    Modulename      = $moduleName
    TemplatePath    = "C:\Repos\win-scripts\PlasterTemplate"
    DestinationPath = "C:\wpe\modules\$moduleName"
    TemplateAuthor  = 'Raj Balgobin'
    Version         = '0.0.1'
}

New-Item -ItemType Directory -Path $plaster.DestinationPath

Invoke-Plaster @plaster -Verbose