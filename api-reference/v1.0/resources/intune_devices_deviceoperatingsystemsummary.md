# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="5e113-101">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="5e113-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="5e113-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e113-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e113-103">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e113-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="5e113-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e113-104">Properties</span></span>
|<span data-ttu-id="5e113-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e113-105">Property</span></span>|<span data-ttu-id="5e113-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e113-106">Type</span></span>|<span data-ttu-id="5e113-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e113-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e113-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="5e113-108">androidCount</span></span>|<span data-ttu-id="5e113-109">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-109">Int32</span></span>|<span data-ttu-id="5e113-110">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="5e113-110">Number of android device count.</span></span>|
|<span data-ttu-id="5e113-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="5e113-111">iosCount</span></span>|<span data-ttu-id="5e113-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-112">Int32</span></span>|<span data-ttu-id="5e113-113">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="5e113-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="5e113-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="5e113-114">macOSCount</span></span>|<span data-ttu-id="5e113-115">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-115">Int32</span></span>|<span data-ttu-id="5e113-116">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="5e113-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="5e113-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="5e113-117">windowsMobileCount</span></span>|<span data-ttu-id="5e113-118">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-118">Int32</span></span>|<span data-ttu-id="5e113-119">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="5e113-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="5e113-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="5e113-120">windowsCount</span></span>|<span data-ttu-id="5e113-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-121">Int32</span></span>|<span data-ttu-id="5e113-122">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="5e113-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="5e113-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="5e113-123">unknownCount</span></span>|<span data-ttu-id="5e113-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5e113-124">Int32</span></span>|<span data-ttu-id="5e113-125">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="5e113-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e113-126">Relações</span><span class="sxs-lookup"><span data-stu-id="5e113-126">Relationships</span></span>
<span data-ttu-id="5e113-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e113-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e113-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e113-128">JSON Representation</span></span>
<span data-ttu-id="5e113-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e113-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```








