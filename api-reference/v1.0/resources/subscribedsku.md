# <a name="subscribedsku-resource-type"></a><span data-ttu-id="d649a-101">Tipo de recurso subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d649a-101">subscribedSku resource type</span></span>

<span data-ttu-id="d649a-102">Contém informações sobre um serviço SKU assinado por uma empresa.</span><span class="sxs-lookup"><span data-stu-id="d649a-102">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="d649a-p101">Somente a operação de leitura é compatível com as SKUs inscritas; criar, atualizar e excluir não têm suporte. Não há suporte para expressões de filtro de consulta. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d649a-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d649a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d649a-106">Methods</span></span>
| <span data-ttu-id="d649a-107">Método</span><span class="sxs-lookup"><span data-stu-id="d649a-107">Method</span></span>           | <span data-ttu-id="d649a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d649a-108">Return Type</span></span>    |<span data-ttu-id="d649a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d649a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d649a-110">Get subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d649a-110">Get subscribedSku</span></span>](../api/subscribedsku_get.md) | [<span data-ttu-id="d649a-111">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d649a-111">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="d649a-112">Leia as propriedades e os relacionamentos do objeto subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="d649a-112">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="d649a-113">Lista subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d649a-113">List subscribedSku</span></span>](../api/subscribedsku_list.md) | <span data-ttu-id="d649a-114">Coleção [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="d649a-114">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="d649a-115">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="d649a-115">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="d649a-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d649a-116">Properties</span></span>
| <span data-ttu-id="d649a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d649a-117">Property</span></span>     | <span data-ttu-id="d649a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d649a-118">Type</span></span>   |<span data-ttu-id="d649a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d649a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d649a-120">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d649a-120">appliesTo</span></span>|<span data-ttu-id="d649a-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d649a-121">String</span></span>| <span data-ttu-id="d649a-122">Por exemplo, “Usuário” ou “Empresa”.</span><span class="sxs-lookup"><span data-stu-id="d649a-122">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="d649a-123">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="d649a-123">capabilityStatus</span></span>|<span data-ttu-id="d649a-124">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d649a-124">String</span></span>| <span data-ttu-id="d649a-125">Por exemplo, “Enabled”.</span><span class="sxs-lookup"><span data-stu-id="d649a-125">For example, "Enabled".</span></span> |
|<span data-ttu-id="d649a-126">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="d649a-126">consumedUnits</span></span>|<span data-ttu-id="d649a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d649a-127">Int32</span></span>| <span data-ttu-id="d649a-128">O número de licenças que foram atribuídas.</span><span class="sxs-lookup"><span data-stu-id="d649a-128">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="d649a-129">id</span><span class="sxs-lookup"><span data-stu-id="d649a-129">id</span></span>|<span data-ttu-id="d649a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d649a-130">String</span></span>| <span data-ttu-id="d649a-p102">O identificador exclusivo do objeto SKU assinado. Chave, não anulável.</span><span class="sxs-lookup"><span data-stu-id="d649a-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="d649a-133">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="d649a-133">prepaidUnits</span></span>|[<span data-ttu-id="d649a-134">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="d649a-134">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="d649a-135">Informações sobre o número e o status das licenças pré-pagas.</span><span class="sxs-lookup"><span data-stu-id="d649a-135">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="d649a-136">servicePlans</span><span class="sxs-lookup"><span data-stu-id="d649a-136">servicePlans</span></span>|<span data-ttu-id="d649a-137">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="d649a-137">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="d649a-p103">Informações sobre os planos do serviço que estão disponíveis com o SKU. Não anulável</span><span class="sxs-lookup"><span data-stu-id="d649a-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="d649a-140">skuId</span><span class="sxs-lookup"><span data-stu-id="d649a-140">skuId</span></span>|<span data-ttu-id="d649a-141">Guid</span><span class="sxs-lookup"><span data-stu-id="d649a-141">Guid</span></span>| <span data-ttu-id="d649a-142">O identificador exclusivo (GUID) do SKU do serviço.</span><span class="sxs-lookup"><span data-stu-id="d649a-142">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="d649a-143">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="d649a-143">skuPartNumber</span></span>|<span data-ttu-id="d649a-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d649a-144">String</span></span>| <span data-ttu-id="d649a-145">O número de peça do SKU, por exemplo: "AAD_PREMIUM" ou "RMSBASIC".</span><span class="sxs-lookup"><span data-stu-id="d649a-145">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="d649a-146">Relações</span><span class="sxs-lookup"><span data-stu-id="d649a-146">Relationships</span></span>
<span data-ttu-id="d649a-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d649a-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d649a-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d649a-148">JSON representation</span></span>

<span data-ttu-id="d649a-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d649a-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
