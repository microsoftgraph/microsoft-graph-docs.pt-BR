# <a name="serviceplaninfo-resource-type"></a><span data-ttu-id="d498f-101">Tipo de recurso servicePlanInfo</span><span class="sxs-lookup"><span data-stu-id="d498f-101">servicePlanInfo resource type</span></span>

<span data-ttu-id="d498f-p101">Contém informações sobre um plano de serviço associado a uma SKU inscrita. A propriedade **servicePlans** da entidade [subscribedSku](subscribedsku.md) é uma coleção de **servicePlanInfo**.</span><span class="sxs-lookup"><span data-stu-id="d498f-p101">Contains information about a service plan associated with a subscribed SKU. The **servicePlans** property of the [subscribedSku](subscribedsku.md) entity is a collection of **servicePlanInfo**.</span></span>


## <a name="properties"></a><span data-ttu-id="d498f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d498f-104">Properties</span></span>
| <span data-ttu-id="d498f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d498f-105">Property</span></span>     | <span data-ttu-id="d498f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d498f-106">Type</span></span>   |<span data-ttu-id="d498f-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d498f-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d498f-108">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="d498f-108">servicePlanId</span></span>|<span data-ttu-id="d498f-109">Guid</span><span class="sxs-lookup"><span data-stu-id="d498f-109">Guid</span></span>|<span data-ttu-id="d498f-110">O identificador exclusivo do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="d498f-110">The unique identifier of the service plan.</span></span>|
|<span data-ttu-id="d498f-111">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="d498f-111">servicePlanName</span></span>|<span data-ttu-id="d498f-112">String</span><span class="sxs-lookup"><span data-stu-id="d498f-112">String</span></span>|<span data-ttu-id="d498f-113">O nome do plano de serviços.</span><span class="sxs-lookup"><span data-stu-id="d498f-113">The name of the service plan.</span></span>|
|<span data-ttu-id="d498f-114">provisioningStatus</span><span class="sxs-lookup"><span data-stu-id="d498f-114">provisioningStatus</span></span>|<span data-ttu-id="d498f-115">String</span><span class="sxs-lookup"><span data-stu-id="d498f-115">String</span></span>|<span data-ttu-id="d498f-p102">O status de provisionamento do plano de serviços. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="d498f-p102">The provisioning status of the service plan. Possible values:</span></span><br/><span data-ttu-id="d498f-118">"Success" – o serviço está totalmente provisionado.</span><span class="sxs-lookup"><span data-stu-id="d498f-118">"Success" - Service is fully provisioned.</span></span><br/><span data-ttu-id="d498f-119">“Disabled” – o serviço foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="d498f-119">"Disabled" - Service has been disabled.</span></span><br/><span data-ttu-id="d498f-120">"PendingInput" – o serviço ainda não está provisionado; aguardando confirmação do serviço.</span><span class="sxs-lookup"><span data-stu-id="d498f-120">"PendingInput" - Service is not yet provisioned; awaiting service confirmation.</span></span><br/><span data-ttu-id="d498f-121">"PendingActivation" – o serviço está provisionado, mas requer ativação explícita pelo administrador (por exemplo, plano de serviço do Intune_O365)</span><span class="sxs-lookup"><span data-stu-id="d498f-121">"PendingActivation" - Service is provisioned but requires explicit activation by administrator (for example, Intune_O365 service plan)</span></span><br/><span data-ttu-id="d498f-122">"PendingProvisioning" – a Microsoft adicionou um novo serviço ao SKU do produto e ele não foi ativado no locatário ainda.</span><span class="sxs-lookup"><span data-stu-id="d498f-122">"PendingProvisioning" - Microsoft has added a new service to the product SKU and it has not been activated in the tenant, yet.</span></span>|
|<span data-ttu-id="d498f-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="d498f-123">appliesTo</span></span>|<span data-ttu-id="d498f-124">String</span><span class="sxs-lookup"><span data-stu-id="d498f-124">String</span></span>|<span data-ttu-id="d498f-p103">O objeto ao qual o plano de serviço pode ser atribuído. Valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="d498f-p103">The object the service plan can be assigned to. Possible values:</span></span><br/><span data-ttu-id="d498f-127">"Usuário" – o plano de serviço pode ser atribuído a usuários individuais.</span><span class="sxs-lookup"><span data-stu-id="d498f-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="d498f-128">"Empresa" – o plano de serviço pode ser atribuído a todos os locatários.</span><span class="sxs-lookup"><span data-stu-id="d498f-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d498f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d498f-129">JSON representation</span></span>

<span data-ttu-id="d498f-130">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d498f-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
