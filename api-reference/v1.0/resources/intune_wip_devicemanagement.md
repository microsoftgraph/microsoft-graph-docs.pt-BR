# <a name="devicemanagement-resource-type"></a><span data-ttu-id="151d5-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="151d5-101">deviceManagement resource type</span></span>

> <span data-ttu-id="151d5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="151d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="151d5-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="151d5-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="151d5-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="151d5-104">Methods</span></span>
|<span data-ttu-id="151d5-105">Método</span><span class="sxs-lookup"><span data-stu-id="151d5-105">Method</span></span>|<span data-ttu-id="151d5-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="151d5-106">Return Type</span></span>|<span data-ttu-id="151d5-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="151d5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="151d5-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="151d5-108">Get deviceManagement</span></span>](../api/intune_wip_devicemanagement_get.md)|[<span data-ttu-id="151d5-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="151d5-109">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="151d5-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_wip_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="151d5-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_wip_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="151d5-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="151d5-111">Update deviceManagement</span></span>](../api/intune_wip_devicemanagement_update.md)|[<span data-ttu-id="151d5-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="151d5-112">deviceManagement</span></span>](../resources/intune_wip_devicemanagement.md)|<span data-ttu-id="151d5-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_wip_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="151d5-113">Update the properties of a [calendar](../resources/intune_wip_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="151d5-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="151d5-114">Properties</span></span>
|<span data-ttu-id="151d5-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="151d5-115">Property</span></span>|<span data-ttu-id="151d5-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="151d5-116">Type</span></span>|<span data-ttu-id="151d5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="151d5-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151d5-118">id</span><span class="sxs-lookup"><span data-stu-id="151d5-118">id</span></span>|<span data-ttu-id="151d5-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="151d5-119">String</span></span>|<span data-ttu-id="151d5-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="151d5-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="151d5-121">Relações</span><span class="sxs-lookup"><span data-stu-id="151d5-121">Relationships</span></span>
|<span data-ttu-id="151d5-122">Relação</span><span class="sxs-lookup"><span data-stu-id="151d5-122">Relationship</span></span>|<span data-ttu-id="151d5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="151d5-123">Type</span></span>|<span data-ttu-id="151d5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="151d5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151d5-125">windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="151d5-125">windowsInformationProtectionAppLearningSummaries</span></span>|<span data-ttu-id="151d5-126">Conjunto [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)</span><span class="sxs-lookup"><span data-stu-id="151d5-126">[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) collection</span></span>|<span data-ttu-id="151d5-127">Os resumos de aprendizagem de aplicativos da proteção de informações do Windows.</span><span class="sxs-lookup"><span data-stu-id="151d5-127">The windows information protection app learning summaries.</span></span>|
|<span data-ttu-id="151d5-128">windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="151d5-128">windowsInformationProtectionNetworkLearningSummaries</span></span>|<span data-ttu-id="151d5-129">Conjunto [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)</span><span class="sxs-lookup"><span data-stu-id="151d5-129">[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) collection</span></span>|<span data-ttu-id="151d5-130">Os resumos de aprendizagem de redes da proteção de informações do Windows.</span><span class="sxs-lookup"><span data-stu-id="151d5-130">The windows information protection network learning summaries.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="151d5-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="151d5-131">JSON Representation</span></span>
<span data-ttu-id="151d5-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="151d5-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



