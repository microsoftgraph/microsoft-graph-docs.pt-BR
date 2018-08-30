# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="213a0-101">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="213a0-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="213a0-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="213a0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="213a0-103">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="213a0-103">Reset passcode action result</span></span>

<span data-ttu-id="213a0-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="213a0-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="213a0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="213a0-105">Properties</span></span>
|<span data-ttu-id="213a0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="213a0-106">Property</span></span>|<span data-ttu-id="213a0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="213a0-107">Type</span></span>|<span data-ttu-id="213a0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="213a0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="213a0-109">actionName</span><span class="sxs-lookup"><span data-stu-id="213a0-109">actionName</span></span>|<span data-ttu-id="213a0-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="213a0-110">String</span></span>|<span data-ttu-id="213a0-111">Nome da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="213a0-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="213a0-112">actionState</span><span class="sxs-lookup"><span data-stu-id="213a0-112">actionState</span></span>|[<span data-ttu-id="213a0-113">actionState</span><span class="sxs-lookup"><span data-stu-id="213a0-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="213a0-114">Estado da ação herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="213a0-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="213a0-115">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="213a0-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="213a0-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="213a0-116">startDateTime</span></span>|<span data-ttu-id="213a0-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="213a0-117">DateTimeOffset</span></span>|<span data-ttu-id="213a0-118">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="213a0-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="213a0-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="213a0-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="213a0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="213a0-120">DateTimeOffset</span></span>|<span data-ttu-id="213a0-121">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="213a0-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="213a0-122">senha</span><span class="sxs-lookup"><span data-stu-id="213a0-122">passcode</span></span>|<span data-ttu-id="213a0-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="213a0-123">String</span></span>|<span data-ttu-id="213a0-124">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="213a0-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="213a0-125">Relações</span><span class="sxs-lookup"><span data-stu-id="213a0-125">Relationships</span></span>
<span data-ttu-id="213a0-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="213a0-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="213a0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="213a0-127">JSON Representation</span></span>
<span data-ttu-id="213a0-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="213a0-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



