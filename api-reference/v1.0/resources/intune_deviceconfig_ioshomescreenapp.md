# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="0dc2e-101">Tipo de recurso iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="0dc2e-101">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="0dc2e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0dc2e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0dc2e-103">Representa um ícone de um aplicativo na tela inicial</span><span class="sxs-lookup"><span data-stu-id="0dc2e-103">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="0dc2e-104">Herda de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dc2e-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0dc2e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0dc2e-105">Properties</span></span>
|<span data-ttu-id="0dc2e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dc2e-106">Property</span></span>|<span data-ttu-id="0dc2e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dc2e-107">Type</span></span>|<span data-ttu-id="0dc2e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dc2e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dc2e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0dc2e-109">displayName</span></span>|<span data-ttu-id="0dc2e-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dc2e-110">String</span></span>|<span data-ttu-id="0dc2e-111">Nome do aplicativo Herdado de [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0dc2e-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="0dc2e-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="0dc2e-112">bundleID</span></span>|<span data-ttu-id="0dc2e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0dc2e-113">String</span></span>|<span data-ttu-id="0dc2e-114">BundleID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dc2e-114">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dc2e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="0dc2e-115">Relationships</span></span>
<span data-ttu-id="0dc2e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0dc2e-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0dc2e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0dc2e-117">JSON Representation</span></span>
<span data-ttu-id="0dc2e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0dc2e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



