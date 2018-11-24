# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="3e948-101">Tipo de recurso updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="3e948-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="3e948-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e948-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e948-103">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3e948-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e948-104">Properties</span></span>
|<span data-ttu-id="3e948-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e948-105">Property</span></span>|<span data-ttu-id="3e948-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e948-106">Type</span></span>|<span data-ttu-id="3e948-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e948-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e948-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="3e948-108">deviceAccount</span></span>|[<span data-ttu-id="3e948-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="3e948-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="3e948-110">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-110">Not yet documented</span></span>|
|<span data-ttu-id="3e948-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="3e948-111">passwordRotationEnabled</span></span>|<span data-ttu-id="3e948-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e948-112">Boolean</span></span>|<span data-ttu-id="3e948-113">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-113">Not yet documented</span></span>|
|<span data-ttu-id="3e948-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="3e948-114">calendarSyncEnabled</span></span>|<span data-ttu-id="3e948-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e948-115">Boolean</span></span>|<span data-ttu-id="3e948-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-116">Not yet documented</span></span>|
|<span data-ttu-id="3e948-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="3e948-117">deviceAccountEmail</span></span>|<span data-ttu-id="3e948-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e948-118">String</span></span>|<span data-ttu-id="3e948-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-119">Not yet documented</span></span>|
|<span data-ttu-id="3e948-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="3e948-120">exchangeServer</span></span>|<span data-ttu-id="3e948-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e948-121">String</span></span>|<span data-ttu-id="3e948-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-122">Not yet documented</span></span>|
|<span data-ttu-id="3e948-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="3e948-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="3e948-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e948-124">String</span></span>|<span data-ttu-id="3e948-125">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e948-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e948-126">Relações</span><span class="sxs-lookup"><span data-stu-id="3e948-126">Relationships</span></span>
<span data-ttu-id="3e948-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e948-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e948-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e948-128">JSON Representation</span></span>
<span data-ttu-id="3e948-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e948-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
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



