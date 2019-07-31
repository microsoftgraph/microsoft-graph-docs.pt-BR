---
title: tipo de recurso licenseDetails
description: Contém informações sobre uma licença atribuída a um usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 12e0dcb86288eb27859b87a1029e89676a5d511b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966953"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="4a8b6-103">tipo de recurso licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4a8b6-103">licenseDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a8b6-104">Contém informações sobre uma licença atribuída a um usuário.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="4a8b6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4a8b6-105">Methods</span></span>

| <span data-ttu-id="4a8b6-106">Método</span><span class="sxs-lookup"><span data-stu-id="4a8b6-106">Method</span></span>           | <span data-ttu-id="4a8b6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4a8b6-107">Return Type</span></span>    |<span data-ttu-id="4a8b6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8b6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a8b6-109">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4a8b6-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="4a8b6-110">Coleção licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4a8b6-110">licenseDetails collection</span></span> |<span data-ttu-id="4a8b6-111">Recupere uma lista de objetos licenseDetails para um usuário.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="4a8b6-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a8b6-112">Properties</span></span>
| <span data-ttu-id="4a8b6-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a8b6-113">Property</span></span>     | <span data-ttu-id="4a8b6-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a8b6-114">Type</span></span>   |<span data-ttu-id="4a8b6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a8b6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a8b6-116">id</span><span class="sxs-lookup"><span data-stu-id="4a8b6-116">id</span></span>|<span data-ttu-id="4a8b6-117">String</span><span class="sxs-lookup"><span data-stu-id="4a8b6-117">String</span></span>| <span data-ttu-id="4a8b6-118">O identificador exclusivo do objeto de detalhes da licença.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="4a8b6-119">Somente leitura, chave, não anulável</span><span class="sxs-lookup"><span data-stu-id="4a8b6-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="4a8b6-120">onplans</span><span class="sxs-lookup"><span data-stu-id="4a8b6-120">servicePlans</span></span>|<span data-ttu-id="4a8b6-121">Coleção [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="4a8b6-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="4a8b6-122">Informações sobre os planos de serviço atribuídos com a licença.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="4a8b6-123">Somente leitura, não nulo</span><span class="sxs-lookup"><span data-stu-id="4a8b6-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="4a8b6-124">skuId</span><span class="sxs-lookup"><span data-stu-id="4a8b6-124">skuId</span></span>|<span data-ttu-id="4a8b6-125">Guid</span><span class="sxs-lookup"><span data-stu-id="4a8b6-125">Guid</span></span>| <span data-ttu-id="4a8b6-126">Identificador exclusivo (GUID) do serviço SKU.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="4a8b6-127">Igual à propriedade skuId no objeto [SubscribedSku](subscribedsku.md) relacionado.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="4a8b6-128">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4a8b6-128">Read-only</span></span> |
|<span data-ttu-id="4a8b6-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="4a8b6-129">skuPartNumber</span></span>|<span data-ttu-id="4a8b6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a8b6-130">String</span></span>| <span data-ttu-id="4a8b6-131">Nome de exibição SKU exclusivo.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-131">Unique SKU display name.</span></span> <span data-ttu-id="4a8b6-132">Igual ao skuPartNumber no objeto [SubscribedSku](subscribedsku.md) relacionado; por exemplo: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="4a8b6-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="4a8b6-133">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="4a8b6-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="4a8b6-134">Relações</span><span class="sxs-lookup"><span data-stu-id="4a8b6-134">Relationships</span></span>
<span data-ttu-id="4a8b6-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a8b6-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a8b6-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a8b6-136">JSON representation</span></span>
<span data-ttu-id="4a8b6-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a8b6-137">Here is a JSON representation of the resource.</span></span>

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
