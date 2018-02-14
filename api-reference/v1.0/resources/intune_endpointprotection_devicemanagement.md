# <a name="devicemanagement-resource-type"></a><span data-ttu-id="aaf7b-101">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aaf7b-101">deviceManagement resource type</span></span>

> <span data-ttu-id="aaf7b-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="aaf7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaf7b-103">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="aaf7b-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="aaf7b-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="aaf7b-104">Methods</span></span>
|<span data-ttu-id="aaf7b-105">Método</span><span class="sxs-lookup"><span data-stu-id="aaf7b-105">Method</span></span>|<span data-ttu-id="aaf7b-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aaf7b-106">Return Type</span></span>|<span data-ttu-id="aaf7b-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaf7b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aaf7b-108">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aaf7b-108">Get deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_get.md)|[<span data-ttu-id="aaf7b-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aaf7b-109">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="aaf7b-110">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune_endpointprotection_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="aaf7b-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="aaf7b-111">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aaf7b-111">Update deviceManagement</span></span>](../api/intune_endpointprotection_devicemanagement_update.md)|[<span data-ttu-id="aaf7b-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="aaf7b-112">deviceManagement</span></span>](../resources/intune_endpointprotection_devicemanagement.md)|<span data-ttu-id="aaf7b-113">Atualize as propriedades de um objeto [deviceManagement](../resources/intune_endpointprotection_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="aaf7b-113">Update the properties of a [calendar](../resources/intune_endpointprotection_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aaf7b-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aaf7b-114">Properties</span></span>
|<span data-ttu-id="aaf7b-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaf7b-115">Property</span></span>|<span data-ttu-id="aaf7b-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaf7b-116">Type</span></span>|<span data-ttu-id="aaf7b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaf7b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf7b-118">id</span><span class="sxs-lookup"><span data-stu-id="aaf7b-118">id</span></span>|<span data-ttu-id="aaf7b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aaf7b-119">String</span></span>|<span data-ttu-id="aaf7b-120">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="aaf7b-120">Unique Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaf7b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="aaf7b-121">Relationships</span></span>
<span data-ttu-id="aaf7b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aaf7b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aaf7b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aaf7b-123">JSON Representation</span></span>
<span data-ttu-id="aaf7b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aaf7b-124">Here is a JSON representation of the resource.</span></span>
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



