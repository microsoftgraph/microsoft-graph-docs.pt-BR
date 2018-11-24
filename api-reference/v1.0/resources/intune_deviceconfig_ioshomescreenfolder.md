# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="9b7ad-101">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="9b7ad-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="9b7ad-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b7ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b7ad-103">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="9b7ad-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="9b7ad-104">Herda de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b7ad-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b7ad-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b7ad-105">Properties</span></span>
|<span data-ttu-id="9b7ad-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b7ad-106">Property</span></span>|<span data-ttu-id="9b7ad-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b7ad-107">Type</span></span>|<span data-ttu-id="9b7ad-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b7ad-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b7ad-109">displayName</span><span class="sxs-lookup"><span data-stu-id="9b7ad-109">displayName</span></span>|<span data-ttu-id="9b7ad-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ad-110">String</span></span>|<span data-ttu-id="9b7ad-111">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="9b7ad-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="9b7ad-112">páginas</span><span class="sxs-lookup"><span data-stu-id="9b7ad-112">pages</span></span>|<span data-ttu-id="9b7ad-113">Conjunto [iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="9b7ad-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="9b7ad-114">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9b7ad-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="9b7ad-115">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9b7ad-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b7ad-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9b7ad-116">Relationships</span></span>
<span data-ttu-id="9b7ad-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b7ad-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b7ad-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b7ad-118">JSON Representation</span></span>
<span data-ttu-id="9b7ad-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b7ad-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```



