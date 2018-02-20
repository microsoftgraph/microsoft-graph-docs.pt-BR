# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="2aec1-101">Tipo de recurso deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2aec1-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="2aec1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2aec1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2aec1-103">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2aec1-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="2aec1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2aec1-104">Properties</span></span>
|<span data-ttu-id="2aec1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2aec1-105">Property</span></span>|<span data-ttu-id="2aec1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="2aec1-106">Type</span></span>|<span data-ttu-id="2aec1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="2aec1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aec1-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2aec1-108">allowedDeviceCount</span></span>|<span data-ttu-id="2aec1-109">Int32</span><span class="sxs-lookup"><span data-stu-id="2aec1-109">Int32</span></span>|<span data-ttu-id="2aec1-110">Contagem total de dispositivos com Estado de Acesso ao Exchange: Permitido.</span><span class="sxs-lookup"><span data-stu-id="2aec1-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="2aec1-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2aec1-111">blockedDeviceCount</span></span>|<span data-ttu-id="2aec1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2aec1-112">Int32</span></span>|<span data-ttu-id="2aec1-113">Contagem total de dispositivos com Estado de Acesso ao Exchange: Bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2aec1-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="2aec1-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2aec1-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="2aec1-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2aec1-115">Int32</span></span>|<span data-ttu-id="2aec1-116">Contagem total de dispositivos com Estado de Acesso ao Exchange: Em quarentena.</span><span class="sxs-lookup"><span data-stu-id="2aec1-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="2aec1-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2aec1-117">unknownDeviceCount</span></span>|<span data-ttu-id="2aec1-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2aec1-118">Int32</span></span>|<span data-ttu-id="2aec1-119">Contagem total de dispositivos com Estado de Acesso ao Exchange: Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="2aec1-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="2aec1-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2aec1-120">unavailableDeviceCount</span></span>|<span data-ttu-id="2aec1-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2aec1-121">Int32</span></span>|<span data-ttu-id="2aec1-122">Contagem total de dispositivos para os quais nenhum Estado de Acesso ao Exchange pôde ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="2aec1-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aec1-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2aec1-123">Relationships</span></span>
<span data-ttu-id="2aec1-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2aec1-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2aec1-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2aec1-125">JSON Representation</span></span>
<span data-ttu-id="2aec1-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2aec1-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```



