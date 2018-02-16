# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="13e6d-101">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="13e6d-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="13e6d-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13e6d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13e6d-103">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="13e6d-103">Reset passcode action result</span></span>

<span data-ttu-id="13e6d-104">Herda de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="13e6d-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13e6d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13e6d-105">Properties</span></span>
|<span data-ttu-id="13e6d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13e6d-106">Property</span></span>|<span data-ttu-id="13e6d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="13e6d-107">Type</span></span>|<span data-ttu-id="13e6d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e6d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13e6d-109">actionName</span><span class="sxs-lookup"><span data-stu-id="13e6d-109">actionName</span></span>|<span data-ttu-id="13e6d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13e6d-110">String</span></span>|<span data-ttu-id="13e6d-111">Nome da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="13e6d-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="13e6d-112">actionState</span><span class="sxs-lookup"><span data-stu-id="13e6d-112">actionState</span></span>|<span data-ttu-id="13e6d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13e6d-113">String</span></span>|<span data-ttu-id="13e6d-114">Estado da ação Herdado de [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="13e6d-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="13e6d-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="13e6d-115">startDateTime</span></span>|<span data-ttu-id="13e6d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e6d-116">DateTimeOffset</span></span>|<span data-ttu-id="13e6d-117">Hora de início da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="13e6d-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="13e6d-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="13e6d-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="13e6d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e6d-119">DateTimeOffset</span></span>|<span data-ttu-id="13e6d-120">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="13e6d-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="13e6d-121">senha</span><span class="sxs-lookup"><span data-stu-id="13e6d-121">passcode</span></span>|<span data-ttu-id="13e6d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13e6d-122">String</span></span>|<span data-ttu-id="13e6d-123">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="13e6d-123">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="13e6d-124">Relações</span><span class="sxs-lookup"><span data-stu-id="13e6d-124">Relationships</span></span>
<span data-ttu-id="13e6d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13e6d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13e6d-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13e6d-126">JSON Representation</span></span>
<span data-ttu-id="13e6d-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13e6d-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
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



