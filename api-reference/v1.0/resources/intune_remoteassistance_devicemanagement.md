# <a name="devicemanagement-resource-type"></a><span data-ttu-id="c6ba7-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6ba7-101">deviceManagement resource type</span></span>

> <span data-ttu-id="c6ba7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6ba7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6ba7-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="c6ba7-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="c6ba7-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="c6ba7-104">Methods</span></span>
|<span data-ttu-id="c6ba7-105">Método</span><span class="sxs-lookup"><span data-stu-id="c6ba7-105">Method</span></span>|<span data-ttu-id="c6ba7-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6ba7-106">Return Type</span></span>|<span data-ttu-id="c6ba7-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6ba7-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6ba7-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6ba7-108">Get deviceManagement</span></span>](../api/intune_remoteassistance_devicemanagement_get.md)|[<span data-ttu-id="c6ba7-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6ba7-109">deviceManagement</span></span>](../resources/intune_remoteassistance_devicemanagement.md)|<span data-ttu-id="c6ba7-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_remoteassistance_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c6ba7-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_remoteassistance_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="c6ba7-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6ba7-111">Update deviceManagement</span></span>](../api/intune_remoteassistance_devicemanagement_update.md)|[<span data-ttu-id="c6ba7-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c6ba7-112">deviceManagement</span></span>](../resources/intune_remoteassistance_devicemanagement.md)|<span data-ttu-id="c6ba7-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_remoteassistance_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c6ba7-113">Update the properties of a [calendar](../resources/intune_remoteassistance_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6ba7-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6ba7-114">Properties</span></span>
|<span data-ttu-id="c6ba7-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6ba7-115">Property</span></span>|<span data-ttu-id="c6ba7-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6ba7-116">Type</span></span>|<span data-ttu-id="c6ba7-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6ba7-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ba7-118">id</span><span class="sxs-lookup"><span data-stu-id="c6ba7-118">id</span></span>|<span data-ttu-id="c6ba7-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6ba7-119">String</span></span>|<span data-ttu-id="c6ba7-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c6ba7-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6ba7-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c6ba7-121">Relationships</span></span>
|<span data-ttu-id="c6ba7-122">Relação</span><span class="sxs-lookup"><span data-stu-id="c6ba7-122">Relationship</span></span>|<span data-ttu-id="c6ba7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6ba7-123">Type</span></span>|<span data-ttu-id="c6ba7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6ba7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ba7-125">remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="c6ba7-125">remoteAssistancePartners</span></span>|<span data-ttu-id="c6ba7-126">Conjunto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)</span><span class="sxs-lookup"><span data-stu-id="c6ba7-126">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="c6ba7-127">Os parceiros de assistência remota.</span><span class="sxs-lookup"><span data-stu-id="c6ba7-127">The remote assist partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6ba7-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6ba7-128">JSON Representation</span></span>
<span data-ttu-id="c6ba7-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6ba7-129">Here is a JSON representation of the resource.</span></span>
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



