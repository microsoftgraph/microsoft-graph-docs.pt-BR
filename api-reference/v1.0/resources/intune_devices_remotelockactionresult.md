# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="e1c50-101">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="e1c50-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="e1c50-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1c50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1c50-103">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="e1c50-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="e1c50-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1c50-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1c50-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1c50-105">Properties</span></span>
|<span data-ttu-id="e1c50-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1c50-106">Property</span></span>|<span data-ttu-id="e1c50-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1c50-107">Type</span></span>|<span data-ttu-id="e1c50-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1c50-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1c50-109">actionName</span><span class="sxs-lookup"><span data-stu-id="e1c50-109">actionName</span></span>|<span data-ttu-id="e1c50-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1c50-110">String</span></span>|<span data-ttu-id="e1c50-111">Nome da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1c50-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1c50-112">actionState</span><span class="sxs-lookup"><span data-stu-id="e1c50-112">actionState</span></span>|<span data-ttu-id="e1c50-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1c50-113">String</span></span>|<span data-ttu-id="e1c50-114">Estado da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e1c50-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e1c50-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c50-115">startDateTime</span></span>|<span data-ttu-id="e1c50-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c50-116">DateTimeOffset</span></span>|<span data-ttu-id="e1c50-117">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1c50-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1c50-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c50-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="e1c50-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c50-119">DateTimeOffset</span></span>|<span data-ttu-id="e1c50-120">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e1c50-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="e1c50-121">unlockPin</span><span class="sxs-lookup"><span data-stu-id="e1c50-121">unlockPin</span></span>|<span data-ttu-id="e1c50-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1c50-122">String</span></span>|<span data-ttu-id="e1c50-123">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="e1c50-123">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1c50-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e1c50-124">Relationships</span></span>
<span data-ttu-id="e1c50-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e1c50-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1c50-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1c50-126">JSON Representation</span></span>
<span data-ttu-id="e1c50-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1c50-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



