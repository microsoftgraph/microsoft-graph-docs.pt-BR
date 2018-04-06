# <a name="devicemanagement-resource-type"></a><span data-ttu-id="ee5da-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ee5da-101">deviceManagement resource type</span></span>

> <span data-ttu-id="ee5da-102">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee5da-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee5da-103">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee5da-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee5da-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ee5da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee5da-105">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ee5da-105">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="ee5da-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee5da-106">Methods</span></span>
|<span data-ttu-id="ee5da-107">Método</span><span class="sxs-lookup"><span data-stu-id="ee5da-107">Method</span></span>|<span data-ttu-id="ee5da-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee5da-108">Return Type</span></span>|<span data-ttu-id="ee5da-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5da-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee5da-110">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ee5da-110">Get deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_get.md)|[<span data-ttu-id="ee5da-111">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ee5da-111">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ee5da-112">Ler propriedades e relações de objetos de [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ee5da-112">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="ee5da-113">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ee5da-113">Update deviceManagement</span></span>](../api/intune_troubleshooting_devicemanagement_update.md)|[<span data-ttu-id="ee5da-114">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ee5da-114">deviceManagement</span></span>](../resources/intune_troubleshooting_devicemanagement.md)|<span data-ttu-id="ee5da-115">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ee5da-115">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee5da-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee5da-116">Properties</span></span>
|<span data-ttu-id="ee5da-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee5da-117">Property</span></span>|<span data-ttu-id="ee5da-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee5da-118">Type</span></span>|<span data-ttu-id="ee5da-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5da-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee5da-120">id</span><span class="sxs-lookup"><span data-stu-id="ee5da-120">id</span></span>|<span data-ttu-id="ee5da-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee5da-121">String</span></span>|<span data-ttu-id="ee5da-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ee5da-122">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee5da-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ee5da-123">Relationships</span></span>
|<span data-ttu-id="ee5da-124">Relação</span><span class="sxs-lookup"><span data-stu-id="ee5da-124">Relationship</span></span>|<span data-ttu-id="ee5da-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee5da-125">Type</span></span>|<span data-ttu-id="ee5da-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee5da-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee5da-127">troubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="ee5da-127">troubleshootingEvents</span></span>|<span data-ttu-id="ee5da-128">Conjunto [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ee5da-128">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="ee5da-129">A lista de eventos de solução de problemas para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee5da-129">The list of troubleshooting events for the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee5da-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee5da-130">JSON Representation</span></span>
<span data-ttu-id="ee5da-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee5da-131">Here is a JSON representation of the resource.</span></span>
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



