---
title: licenciamentoDeseto de recurso
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4e23dfcd15dc2b05a9d1c7356a532e6faf487662
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547187"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="1d35a-103">licenciamentoDeseto de recurso</span><span class="sxs-lookup"><span data-stu-id="1d35a-103">licenseDetails resource type</span></span>

<span data-ttu-id="1d35a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d35a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d35a-105">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="1d35a-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="1d35a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d35a-106">Methods</span></span>

| <span data-ttu-id="1d35a-107">Método</span><span class="sxs-lookup"><span data-stu-id="1d35a-107">Method</span></span>           | <span data-ttu-id="1d35a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d35a-108">Return Type</span></span>    |<span data-ttu-id="1d35a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d35a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d35a-110">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="1d35a-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="1d35a-111">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="1d35a-111">licenseDetails collection</span></span> |<span data-ttu-id="1d35a-112">Recuperar uma lista de objetos de licençade detalhes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="1d35a-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="1d35a-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d35a-113">Properties</span></span>
| <span data-ttu-id="1d35a-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d35a-114">Property</span></span>     | <span data-ttu-id="1d35a-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d35a-115">Type</span></span>   |<span data-ttu-id="1d35a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d35a-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d35a-117">id</span><span class="sxs-lookup"><span data-stu-id="1d35a-117">id</span></span>|<span data-ttu-id="1d35a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d35a-118">String</span></span>| <span data-ttu-id="1d35a-119">O identificador exclusivo para o objeto de detalhe de licença.</span><span class="sxs-lookup"><span data-stu-id="1d35a-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="1d35a-120">Somente leitura, chave, não é nulo</span><span class="sxs-lookup"><span data-stu-id="1d35a-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="1d35a-121">planos de serviço</span><span class="sxs-lookup"><span data-stu-id="1d35a-121">servicePlans</span></span>|<span data-ttu-id="1d35a-122">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="1d35a-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="1d35a-123">Informações sobre os planos de serviço atribuídos à licença.</span><span class="sxs-lookup"><span data-stu-id="1d35a-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="1d35a-124">Somente leitura, não é nulo</span><span class="sxs-lookup"><span data-stu-id="1d35a-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="1d35a-125">skuId</span><span class="sxs-lookup"><span data-stu-id="1d35a-125">skuId</span></span>|<span data-ttu-id="1d35a-126">Guid</span><span class="sxs-lookup"><span data-stu-id="1d35a-126">Guid</span></span>| <span data-ttu-id="1d35a-127">Identificador exclusivo (GUID) para o serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="1d35a-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="1d35a-128">Igual à propriedade skuId no objeto [AssinadSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="1d35a-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="1d35a-129">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1d35a-129">Read-only</span></span> |
|<span data-ttu-id="1d35a-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="1d35a-130">skuPartNumber</span></span>|<span data-ttu-id="1d35a-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d35a-131">String</span></span>| <span data-ttu-id="1d35a-132">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="1d35a-132">Unique SKU display name.</span></span> <span data-ttu-id="1d35a-133">Igual ao skuPartNumber no objeto [AssinadSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="1d35a-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="1d35a-134">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="1d35a-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d35a-135">Relações</span><span class="sxs-lookup"><span data-stu-id="1d35a-135">Relationships</span></span>
<span data-ttu-id="1d35a-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d35a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d35a-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d35a-137">JSON representation</span></span>
<span data-ttu-id="1d35a-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d35a-138">Here is a JSON representation of the resource.</span></span>

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

