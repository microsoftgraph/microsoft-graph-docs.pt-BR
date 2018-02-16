# <a name="devicemanagement-resource-type"></a><span data-ttu-id="ea356-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ea356-101">deviceManagement resource type</span></span>

> <span data-ttu-id="ea356-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea356-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea356-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ea356-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="ea356-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea356-104">Methods</span></span>
|<span data-ttu-id="ea356-105">Método</span><span class="sxs-lookup"><span data-stu-id="ea356-105">Method</span></span>|<span data-ttu-id="ea356-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea356-106">Return Type</span></span>|<span data-ttu-id="ea356-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea356-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea356-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ea356-108">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="ea356-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ea356-109">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ea356-110">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ea356-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="ea356-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ea356-111">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="ea356-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ea356-112">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ea356-113">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ea356-113">Update the properties of a [calendar](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea356-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea356-114">Properties</span></span>
|<span data-ttu-id="ea356-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea356-115">Property</span></span>|<span data-ttu-id="ea356-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea356-116">Type</span></span>|<span data-ttu-id="ea356-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea356-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea356-118">id</span><span class="sxs-lookup"><span data-stu-id="ea356-118">id</span></span>|<span data-ttu-id="ea356-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea356-119">String</span></span>|<span data-ttu-id="ea356-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ea356-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea356-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ea356-121">Relationships</span></span>
|<span data-ttu-id="ea356-122">Relação</span><span class="sxs-lookup"><span data-stu-id="ea356-122">Relationship</span></span>|<span data-ttu-id="ea356-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea356-123">Type</span></span>|<span data-ttu-id="ea356-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea356-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea356-125">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="ea356-125">troubleshootingEvents</span></span>|<span data-ttu-id="ea356-126">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ea356-126">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="ea356-127">A lista de eventos de solução de problemas para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea356-127">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea356-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea356-128">JSON Representation</span></span>
<span data-ttu-id="ea356-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea356-129">Here is a JSON representation of the resource.</span></span>
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



