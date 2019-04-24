---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
ms.openlocfilehash: 4495e85b45f6fcfda4f37e467e9cdc5393787dc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585185"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="9deed-103">tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="9deed-103">licenseDetails resource type</span></span>

<span data-ttu-id="9deed-104">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="9deed-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="9deed-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9deed-105">Methods</span></span>

| <span data-ttu-id="9deed-106">Método</span><span class="sxs-lookup"><span data-stu-id="9deed-106">Method</span></span>           | <span data-ttu-id="9deed-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9deed-107">Return Type</span></span>    |<span data-ttu-id="9deed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9deed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9deed-109">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="9deed-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="9deed-110">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="9deed-110">licenseDetails collection</span></span> |<span data-ttu-id="9deed-111">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="9deed-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="9deed-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9deed-112">Properties</span></span>
| <span data-ttu-id="9deed-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9deed-113">Property</span></span>     | <span data-ttu-id="9deed-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9deed-114">Type</span></span>   |<span data-ttu-id="9deed-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9deed-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9deed-116">id</span><span class="sxs-lookup"><span data-stu-id="9deed-116">id</span></span>|<span data-ttu-id="9deed-117">String</span><span class="sxs-lookup"><span data-stu-id="9deed-117">String</span></span>| <span data-ttu-id="9deed-118">O identificador exclusivo do objeto de detalhes da licença.</span><span class="sxs-lookup"><span data-stu-id="9deed-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="9deed-119">Somente leitura, chave, não anulável</span><span class="sxs-lookup"><span data-stu-id="9deed-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="9deed-120">onPlans</span><span class="sxs-lookup"><span data-stu-id="9deed-120">servicePlans</span></span>|<span data-ttu-id="9deed-121">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="9deed-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="9deed-122">Informações sobre os planos de serviço atribuídos com a licença.</span><span class="sxs-lookup"><span data-stu-id="9deed-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="9deed-123">Somente leitura, não nulo</span><span class="sxs-lookup"><span data-stu-id="9deed-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="9deed-124">skuId</span><span class="sxs-lookup"><span data-stu-id="9deed-124">skuId</span></span>|<span data-ttu-id="9deed-125">Guid</span><span class="sxs-lookup"><span data-stu-id="9deed-125">Guid</span></span>| <span data-ttu-id="9deed-126">Identificador exclusivo (GUID) do serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="9deed-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="9deed-127">Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="9deed-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="9deed-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9deed-128">Read-only</span></span> |
|<span data-ttu-id="9deed-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="9deed-129">skuPartNumber</span></span>|<span data-ttu-id="9deed-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9deed-130">String</span></span>| <span data-ttu-id="9deed-131">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="9deed-131">Unique SKU display name.</span></span> <span data-ttu-id="9deed-132">Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="9deed-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="9deed-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="9deed-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="9deed-134">Relações</span><span class="sxs-lookup"><span data-stu-id="9deed-134">Relationships</span></span>
<span data-ttu-id="9deed-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9deed-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9deed-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9deed-136">JSON representation</span></span>
<span data-ttu-id="9deed-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9deed-137">Here is a JSON representation of the resource.</span></span>

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
