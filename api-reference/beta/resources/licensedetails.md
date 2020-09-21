---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5236a73697ea6969698fa0cdb6a8368188d0271c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029194"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="38a09-103">tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="38a09-103">licenseDetails resource type</span></span>

<span data-ttu-id="38a09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a09-105">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="38a09-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="38a09-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="38a09-106">Methods</span></span>

| <span data-ttu-id="38a09-107">Método</span><span class="sxs-lookup"><span data-stu-id="38a09-107">Method</span></span>           | <span data-ttu-id="38a09-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38a09-108">Return Type</span></span>    |<span data-ttu-id="38a09-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a09-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38a09-110">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="38a09-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="38a09-111">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="38a09-111">licenseDetails collection</span></span> |<span data-ttu-id="38a09-112">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="38a09-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="38a09-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38a09-113">Properties</span></span>
| <span data-ttu-id="38a09-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38a09-114">Property</span></span>     | <span data-ttu-id="38a09-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="38a09-115">Type</span></span>   |<span data-ttu-id="38a09-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a09-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a09-117">id</span><span class="sxs-lookup"><span data-stu-id="38a09-117">id</span></span>|<span data-ttu-id="38a09-118">String</span><span class="sxs-lookup"><span data-stu-id="38a09-118">String</span></span>| <span data-ttu-id="38a09-119">O identificador exclusivo do objeto de detalhes da licença.</span><span class="sxs-lookup"><span data-stu-id="38a09-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="38a09-120">Somente leitura, chave, não anulável</span><span class="sxs-lookup"><span data-stu-id="38a09-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="38a09-121">onplans</span><span class="sxs-lookup"><span data-stu-id="38a09-121">servicePlans</span></span>|<span data-ttu-id="38a09-122">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="38a09-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="38a09-123">Informações sobre os planos de serviço atribuídos com a licença.</span><span class="sxs-lookup"><span data-stu-id="38a09-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="38a09-124">Somente leitura, não nulo</span><span class="sxs-lookup"><span data-stu-id="38a09-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="38a09-125">skuId</span><span class="sxs-lookup"><span data-stu-id="38a09-125">skuId</span></span>|<span data-ttu-id="38a09-126">Guid</span><span class="sxs-lookup"><span data-stu-id="38a09-126">Guid</span></span>| <span data-ttu-id="38a09-127">Identificador exclusivo (GUID) do serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="38a09-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="38a09-128">Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="38a09-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="38a09-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="38a09-129">Read-only</span></span> |
|<span data-ttu-id="38a09-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="38a09-130">skuPartNumber</span></span>|<span data-ttu-id="38a09-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38a09-131">String</span></span>| <span data-ttu-id="38a09-132">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="38a09-132">Unique SKU display name.</span></span> <span data-ttu-id="38a09-133">Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="38a09-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="38a09-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="38a09-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="38a09-135">Relações</span><span class="sxs-lookup"><span data-stu-id="38a09-135">Relationships</span></span>
<span data-ttu-id="38a09-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38a09-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38a09-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38a09-137">JSON representation</span></span>
<span data-ttu-id="38a09-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38a09-138">Here is a JSON representation of the resource.</span></span>

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


