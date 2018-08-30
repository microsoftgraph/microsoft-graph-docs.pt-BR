# <a name="licensedetails-resource-type"></a><span data-ttu-id="c5437-101">Tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c5437-101">licenseDetails resource type</span></span>

<span data-ttu-id="c5437-102">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c5437-102">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="c5437-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5437-103">Methods</span></span>

| <span data-ttu-id="c5437-104">Método</span><span class="sxs-lookup"><span data-stu-id="c5437-104">Method</span></span>           | <span data-ttu-id="c5437-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5437-105">Return Type</span></span>    |<span data-ttu-id="c5437-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5437-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5437-107">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c5437-107">List licenseDetails</span></span>](../api/user_list_licensedetails.md) | <span data-ttu-id="c5437-108">coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c5437-108">licenseDetails collection</span></span> |<span data-ttu-id="c5437-109">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="c5437-109">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="c5437-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5437-110">Properties</span></span>
| <span data-ttu-id="c5437-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5437-111">Property</span></span>     | <span data-ttu-id="c5437-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5437-112">Type</span></span>   |<span data-ttu-id="c5437-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5437-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5437-114">id</span><span class="sxs-lookup"><span data-stu-id="c5437-114">id</span></span>|<span data-ttu-id="c5437-115">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5437-115">String</span></span>| <span data-ttu-id="c5437-p101">O identificador exclusivo do objeto de detalhe de licença. Somente leitura, Chave, Não anulável</span><span class="sxs-lookup"><span data-stu-id="c5437-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="c5437-118">servicePlans</span><span class="sxs-lookup"><span data-stu-id="c5437-118">servicePlans</span></span>|<span data-ttu-id="c5437-119">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c5437-119">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c5437-p102">Informações sobre os planos de serviços que estão disponíveis com a licença. Somente leitura, Não anulável</span><span class="sxs-lookup"><span data-stu-id="c5437-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="c5437-122">skuId</span><span class="sxs-lookup"><span data-stu-id="c5437-122">skuId</span></span>|<span data-ttu-id="c5437-123">Guid</span><span class="sxs-lookup"><span data-stu-id="c5437-123">Guid</span></span>| <span data-ttu-id="c5437-p103">O identificador exclusivo (GUID) do SKU do serviço. Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado. Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5437-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="c5437-127">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="c5437-127">skuPartNumber</span></span>|<span data-ttu-id="c5437-128">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5437-128">String</span></span>| <span data-ttu-id="c5437-p104">Nome de exibição exclusivo do SKU. Igual à propriedade skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado. Por exemplo: "AAD_Premium". Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c5437-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="c5437-132">Relações</span><span class="sxs-lookup"><span data-stu-id="c5437-132">Relationships</span></span>
<span data-ttu-id="c5437-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5437-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5437-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5437-134">JSON representation</span></span>
<span data-ttu-id="c5437-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5437-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->