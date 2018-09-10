# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="419d4-101">Tipo de recurso updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="419d4-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="419d4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="419d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="419d4-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="419d4-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="419d4-104">Properties</span></span>
|<span data-ttu-id="419d4-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="419d4-105">Property</span></span>|<span data-ttu-id="419d4-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="419d4-106">Type</span></span>|<span data-ttu-id="419d4-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="419d4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="419d4-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="419d4-108">deviceAccount</span></span>|[<span data-ttu-id="419d4-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="419d4-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="419d4-110">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-110">Not yet documented</span></span>|
|<span data-ttu-id="419d4-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="419d4-111">passwordRotationEnabled</span></span>|<span data-ttu-id="419d4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="419d4-112">Boolean</span></span>|<span data-ttu-id="419d4-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-113">Not yet documented</span></span>|
|<span data-ttu-id="419d4-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="419d4-114">calendarSyncEnabled</span></span>|<span data-ttu-id="419d4-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="419d4-115">Boolean</span></span>|<span data-ttu-id="419d4-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-116">Not yet documented</span></span>|
|<span data-ttu-id="419d4-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="419d4-117">deviceAccountEmail</span></span>|<span data-ttu-id="419d4-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="419d4-118">String</span></span>|<span data-ttu-id="419d4-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-119">Not yet documented</span></span>|
|<span data-ttu-id="419d4-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="419d4-120">exchangeServer</span></span>|<span data-ttu-id="419d4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="419d4-121">String</span></span>|<span data-ttu-id="419d4-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-122">Not yet documented</span></span>|
|<span data-ttu-id="419d4-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="419d4-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="419d4-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="419d4-124">String</span></span>|<span data-ttu-id="419d4-125">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="419d4-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="419d4-126">Relações</span><span class="sxs-lookup"><span data-stu-id="419d4-126">Relationships</span></span>
<span data-ttu-id="419d4-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="419d4-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="419d4-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="419d4-128">JSON Representation</span></span>
<span data-ttu-id="419d4-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="419d4-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```








