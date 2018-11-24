# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="16cae-101">Tipo de recurso iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="16cae-101">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="16cae-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16cae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16cae-103">Uma página que contém aplicativos e pastas na tela inicial</span><span class="sxs-lookup"><span data-stu-id="16cae-103">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="16cae-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16cae-104">Properties</span></span>
|<span data-ttu-id="16cae-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16cae-105">Property</span></span>|<span data-ttu-id="16cae-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="16cae-106">Type</span></span>|<span data-ttu-id="16cae-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="16cae-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16cae-108">displayName</span><span class="sxs-lookup"><span data-stu-id="16cae-108">displayName</span></span>|<span data-ttu-id="16cae-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16cae-109">String</span></span>|<span data-ttu-id="16cae-110">Nome da página</span><span class="sxs-lookup"><span data-stu-id="16cae-110">Name of the page</span></span>|
|<span data-ttu-id="16cae-111">ícones</span><span class="sxs-lookup"><span data-stu-id="16cae-111">icons</span></span>|<span data-ttu-id="16cae-112">Conjunto [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="16cae-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="16cae-113">Uma lista dos aplicativos e pastas exibidos em uma página.</span><span class="sxs-lookup"><span data-stu-id="16cae-113">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="16cae-114">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="16cae-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16cae-115">Relações</span><span class="sxs-lookup"><span data-stu-id="16cae-115">Relationships</span></span>
<span data-ttu-id="16cae-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16cae-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16cae-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16cae-117">JSON Representation</span></span>
<span data-ttu-id="16cae-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16cae-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



