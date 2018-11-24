# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="e1ba7-101">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e1ba7-101">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="e1ba7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1ba7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1ba7-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1ba7-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e1ba7-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1ba7-104">Properties</span></span>
|<span data-ttu-id="e1ba7-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1ba7-105">Property</span></span>|<span data-ttu-id="e1ba7-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ba7-106">Type</span></span>|<span data-ttu-id="e1ba7-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ba7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ba7-108">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="e1ba7-108">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="e1ba7-109">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ba7-109">Int32</span></span>|<span data-ttu-id="e1ba7-110">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="e1ba7-110">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="e1ba7-111">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="e1ba7-111">Valid values 0 to 120</span></span>|
|<span data-ttu-id="e1ba7-112">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="e1ba7-112">isScheduledActionEnabled</span></span>|<span data-ttu-id="e1ba7-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1ba7-113">Boolean</span></span>|<span data-ttu-id="e1ba7-114">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="e1ba7-114">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="e1ba7-115">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="e1ba7-115">secureByDefault</span></span>|<span data-ttu-id="e1ba7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1ba7-116">Boolean</span></span>|<span data-ttu-id="e1ba7-117">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="e1ba7-117">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1ba7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e1ba7-118">Relationships</span></span>
<span data-ttu-id="e1ba7-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e1ba7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1ba7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1ba7-120">JSON Representation</span></span>
<span data-ttu-id="e1ba7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1ba7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



