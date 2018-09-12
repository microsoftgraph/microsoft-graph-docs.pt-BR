# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="0794a-101">Tipo de recurso importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="0794a-101">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="0794a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0794a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0794a-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0794a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0794a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0794a-104">Properties</span></span>
|<span data-ttu-id="0794a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0794a-105">Property</span></span>|<span data-ttu-id="0794a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="0794a-106">Type</span></span>|<span data-ttu-id="0794a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0794a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0794a-108">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="0794a-108">deviceImportStatus</span></span>|[<span data-ttu-id="0794a-109">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="0794a-109">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="0794a-p101">Status do dispositivo relatado pelo Serviço de Diretório do Dispositivo (DDS). Os valores possíveis são: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="0794a-p101">Device status reported by Device Directory Service(DDS). The possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="0794a-112">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0794a-112">deviceRegistrationId</span></span>|<span data-ttu-id="0794a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0794a-113">String</span></span>|<span data-ttu-id="0794a-114">ID de Registro do Dispositivo para dispositivo adicionado com êxito relatada pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="0794a-114">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0794a-115">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="0794a-115">deviceErrorCode</span></span>|<span data-ttu-id="0794a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0794a-116">Int32</span></span>|<span data-ttu-id="0794a-117">Código de erro do dispositivo relatado pelo Device Directory Service (DDS).</span><span class="sxs-lookup"><span data-stu-id="0794a-117">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0794a-118">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="0794a-118">deviceErrorName</span></span>|<span data-ttu-id="0794a-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0794a-119">String</span></span>|<span data-ttu-id="0794a-120">Nome do erro de dispositivo relatado pelo Device Directory Service(DDS).</span><span class="sxs-lookup"><span data-stu-id="0794a-120">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0794a-121">Relações</span><span class="sxs-lookup"><span data-stu-id="0794a-121">Relationships</span></span>
<span data-ttu-id="0794a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0794a-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0794a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0794a-123">JSON Representation</span></span>
<span data-ttu-id="0794a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0794a-124">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```








