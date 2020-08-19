---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6e57be3eb8524dc5edf2d8daf683a45de12601c1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811312"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="aac6c-103">tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="aac6c-103">licenseDetails resource type</span></span>

<span data-ttu-id="aac6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aac6c-105">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="aac6c-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="aac6c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="aac6c-106">Methods</span></span>

| <span data-ttu-id="aac6c-107">Método</span><span class="sxs-lookup"><span data-stu-id="aac6c-107">Method</span></span>           | <span data-ttu-id="aac6c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aac6c-108">Return Type</span></span>    |<span data-ttu-id="aac6c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac6c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aac6c-110">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="aac6c-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="aac6c-111">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="aac6c-111">licenseDetails collection</span></span> |<span data-ttu-id="aac6c-112">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="aac6c-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="aac6c-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aac6c-113">Properties</span></span>
| <span data-ttu-id="aac6c-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aac6c-114">Property</span></span>     | <span data-ttu-id="aac6c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="aac6c-115">Type</span></span>   |<span data-ttu-id="aac6c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac6c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aac6c-117">id</span><span class="sxs-lookup"><span data-stu-id="aac6c-117">id</span></span>|<span data-ttu-id="aac6c-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6c-118">String</span></span>| <span data-ttu-id="aac6c-119">O identificador exclusivo do objeto de detalhes da licença.</span><span class="sxs-lookup"><span data-stu-id="aac6c-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="aac6c-120">Somente leitura, chave, não anulável</span><span class="sxs-lookup"><span data-stu-id="aac6c-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="aac6c-121">onplans</span><span class="sxs-lookup"><span data-stu-id="aac6c-121">servicePlans</span></span>|<span data-ttu-id="aac6c-122">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="aac6c-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="aac6c-123">Informações sobre os planos de serviço atribuídos com a licença.</span><span class="sxs-lookup"><span data-stu-id="aac6c-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="aac6c-124">Somente leitura, não nulo</span><span class="sxs-lookup"><span data-stu-id="aac6c-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="aac6c-125">skuId</span><span class="sxs-lookup"><span data-stu-id="aac6c-125">skuId</span></span>|<span data-ttu-id="aac6c-126">Guid</span><span class="sxs-lookup"><span data-stu-id="aac6c-126">Guid</span></span>| <span data-ttu-id="aac6c-127">Identificador exclusivo (GUID) do serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="aac6c-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="aac6c-128">Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="aac6c-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="aac6c-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="aac6c-129">Read-only</span></span> |
|<span data-ttu-id="aac6c-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="aac6c-130">skuPartNumber</span></span>|<span data-ttu-id="aac6c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac6c-131">String</span></span>| <span data-ttu-id="aac6c-132">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="aac6c-132">Unique SKU display name.</span></span> <span data-ttu-id="aac6c-133">Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="aac6c-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="aac6c-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="aac6c-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="aac6c-135">Relações</span><span class="sxs-lookup"><span data-stu-id="aac6c-135">Relationships</span></span>
<span data-ttu-id="aac6c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aac6c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aac6c-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aac6c-137">JSON representation</span></span>
<span data-ttu-id="aac6c-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aac6c-138">Here is a JSON representation of the resource.</span></span>

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
