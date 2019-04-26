---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
ms.openlocfilehash: 6b977dcff67ac9dc03890a4f2182d8b1d974f314
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345265"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="d3ddf-103">tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="d3ddf-103">licenseDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3ddf-104">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="d3ddf-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d3ddf-105">Methods</span></span>

| <span data-ttu-id="d3ddf-106">Método</span><span class="sxs-lookup"><span data-stu-id="d3ddf-106">Method</span></span>           | <span data-ttu-id="d3ddf-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d3ddf-107">Return Type</span></span>    |<span data-ttu-id="d3ddf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3ddf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3ddf-109">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="d3ddf-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="d3ddf-110">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="d3ddf-110">licenseDetails collection</span></span> |<span data-ttu-id="d3ddf-111">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="d3ddf-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3ddf-112">Properties</span></span>
| <span data-ttu-id="d3ddf-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3ddf-113">Property</span></span>     | <span data-ttu-id="d3ddf-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3ddf-114">Type</span></span>   |<span data-ttu-id="d3ddf-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3ddf-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3ddf-116">id</span><span class="sxs-lookup"><span data-stu-id="d3ddf-116">id</span></span>|<span data-ttu-id="d3ddf-117">String</span><span class="sxs-lookup"><span data-stu-id="d3ddf-117">String</span></span>| <span data-ttu-id="d3ddf-118">O identificador exclusivo do objeto de detalhes da licença.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="d3ddf-119">Somente leitura, chave, não anulável</span><span class="sxs-lookup"><span data-stu-id="d3ddf-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="d3ddf-120">onPlans</span><span class="sxs-lookup"><span data-stu-id="d3ddf-120">servicePlans</span></span>|<span data-ttu-id="d3ddf-121">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="d3ddf-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="d3ddf-122">Informações sobre os planos de serviço atribuídos com a licença.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="d3ddf-123">Somente leitura, não nulo</span><span class="sxs-lookup"><span data-stu-id="d3ddf-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="d3ddf-124">skuId</span><span class="sxs-lookup"><span data-stu-id="d3ddf-124">skuId</span></span>|<span data-ttu-id="d3ddf-125">Guid</span><span class="sxs-lookup"><span data-stu-id="d3ddf-125">Guid</span></span>| <span data-ttu-id="d3ddf-126">Identificador exclusivo (GUID) do serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="d3ddf-127">Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="d3ddf-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="d3ddf-128">Read-only</span></span> |
|<span data-ttu-id="d3ddf-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="d3ddf-129">skuPartNumber</span></span>|<span data-ttu-id="d3ddf-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3ddf-130">String</span></span>| <span data-ttu-id="d3ddf-131">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-131">Unique SKU display name.</span></span> <span data-ttu-id="d3ddf-132">Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="d3ddf-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="d3ddf-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="d3ddf-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3ddf-134">Relações</span><span class="sxs-lookup"><span data-stu-id="d3ddf-134">Relationships</span></span>
<span data-ttu-id="d3ddf-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3ddf-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3ddf-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3ddf-136">JSON representation</span></span>
<span data-ttu-id="d3ddf-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3ddf-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
