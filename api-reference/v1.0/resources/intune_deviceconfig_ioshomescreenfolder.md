# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="25ce0-101">Tipo de recurso iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="25ce0-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="25ce0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="25ce0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25ce0-103">Uma pasta que contém as páginas de aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="25ce0-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="25ce0-104">Herda de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="25ce0-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25ce0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25ce0-105">Properties</span></span>
|<span data-ttu-id="25ce0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25ce0-106">Property</span></span>|<span data-ttu-id="25ce0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="25ce0-107">Type</span></span>|<span data-ttu-id="25ce0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="25ce0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25ce0-109">displayName</span><span class="sxs-lookup"><span data-stu-id="25ce0-109">displayName</span></span>|<span data-ttu-id="25ce0-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25ce0-110">String</span></span>|<span data-ttu-id="25ce0-111">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="25ce0-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="25ce0-112">páginas</span><span class="sxs-lookup"><span data-stu-id="25ce0-112">pages</span></span>|<span data-ttu-id="25ce0-113">Conjunto [iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="25ce0-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="25ce0-114">Páginas de ícones de layout da tela inicial que devem ser do tipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25ce0-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="25ce0-115">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="25ce0-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25ce0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="25ce0-116">Relationships</span></span>
<span data-ttu-id="25ce0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25ce0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="25ce0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25ce0-118">JSON Representation</span></span>
<span data-ttu-id="25ce0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25ce0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



