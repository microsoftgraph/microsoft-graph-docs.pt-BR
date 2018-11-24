# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="66d52-101">Tipo de recurso iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="66d52-101">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="66d52-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="66d52-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66d52-103">O identificador de um aplicativo iOS.</span><span class="sxs-lookup"><span data-stu-id="66d52-103">The identifier for an iOS app.</span></span>

<span data-ttu-id="66d52-104">Herda de [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="66d52-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66d52-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66d52-105">Properties</span></span>
|<span data-ttu-id="66d52-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66d52-106">Property</span></span>|<span data-ttu-id="66d52-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d52-107">Type</span></span>|<span data-ttu-id="66d52-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d52-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d52-109">bundleId</span><span class="sxs-lookup"><span data-stu-id="66d52-109">bundleId</span></span>|<span data-ttu-id="66d52-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66d52-110">String</span></span>|<span data-ttu-id="66d52-111">O identificador de um aplicativo, conforme especificado na App Store.</span><span class="sxs-lookup"><span data-stu-id="66d52-111">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d52-112">Relações</span><span class="sxs-lookup"><span data-stu-id="66d52-112">Relationships</span></span>
<span data-ttu-id="66d52-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66d52-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66d52-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66d52-114">JSON Representation</span></span>
<span data-ttu-id="66d52-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66d52-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



