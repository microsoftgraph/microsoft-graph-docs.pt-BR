# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="b1e6e-101">Tipo de recurso deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="b1e6e-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="b1e6e-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1e6e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1e6e-103">Restrições de registro específicas de plataformas</span><span class="sxs-lookup"><span data-stu-id="b1e6e-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="b1e6e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1e6e-104">Properties</span></span>
|<span data-ttu-id="b1e6e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1e6e-105">Property</span></span>|<span data-ttu-id="b1e6e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1e6e-106">Type</span></span>|<span data-ttu-id="b1e6e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1e6e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1e6e-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="b1e6e-108">platformBlocked</span></span>|<span data-ttu-id="b1e6e-109">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1e6e-109">Boolean</span></span>|<span data-ttu-id="b1e6e-110">Bloqueia o registro da plataforma</span><span class="sxs-lookup"><span data-stu-id="b1e6e-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="b1e6e-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="b1e6e-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="b1e6e-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1e6e-112">Boolean</span></span>|<span data-ttu-id="b1e6e-113">Bloqueia o registro de dispositivos de sua propriedade</span><span class="sxs-lookup"><span data-stu-id="b1e6e-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="b1e6e-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1e6e-114">osMinimumVersion</span></span>|<span data-ttu-id="b1e6e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e6e-115">String</span></span>|<span data-ttu-id="b1e6e-116">Versão do SO mínimo compatível</span><span class="sxs-lookup"><span data-stu-id="b1e6e-116">Min OS version supported</span></span>|
|<span data-ttu-id="b1e6e-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1e6e-117">osMaximumVersion</span></span>|<span data-ttu-id="b1e6e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1e6e-118">String</span></span>|<span data-ttu-id="b1e6e-119">Versão do SO máximo compatível</span><span class="sxs-lookup"><span data-stu-id="b1e6e-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1e6e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b1e6e-120">Relationships</span></span>
<span data-ttu-id="b1e6e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1e6e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1e6e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1e6e-122">JSON Representation</span></span>
<span data-ttu-id="b1e6e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1e6e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



