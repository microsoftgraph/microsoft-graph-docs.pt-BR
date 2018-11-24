# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="706e4-101">Tipo de recurso iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="706e4-101">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="706e4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="706e4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="706e4-103">Uma pasta com os aplicativos na tela inicial</span><span class="sxs-lookup"><span data-stu-id="706e4-103">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="706e4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="706e4-104">Properties</span></span>
|<span data-ttu-id="706e4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="706e4-105">Property</span></span>|<span data-ttu-id="706e4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="706e4-106">Type</span></span>|<span data-ttu-id="706e4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="706e4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="706e4-108">displayName</span><span class="sxs-lookup"><span data-stu-id="706e4-108">displayName</span></span>|<span data-ttu-id="706e4-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="706e4-109">String</span></span>|<span data-ttu-id="706e4-110">Nome da página da pasta</span><span class="sxs-lookup"><span data-stu-id="706e4-110">Name of the folder page</span></span>|
|<span data-ttu-id="706e4-111">aplicativos</span><span class="sxs-lookup"><span data-stu-id="706e4-111">apps</span></span>|<span data-ttu-id="706e4-112">Conjunto [iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="706e4-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="706e4-113">Uma lista de aplicativos exibidos em uma página dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="706e4-113">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="706e4-114">Este conjunto pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="706e4-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="706e4-115">Relações</span><span class="sxs-lookup"><span data-stu-id="706e4-115">Relationships</span></span>
<span data-ttu-id="706e4-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="706e4-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="706e4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="706e4-117">JSON Representation</span></span>
<span data-ttu-id="706e4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="706e4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



