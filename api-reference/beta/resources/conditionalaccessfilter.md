---
title: Tipo de recurso conditionalAccessFilter
description: Representa o filtro no escopo da política.
localization_priority: Normal
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f5b14a3faa593453c88cc155f7e44348fcfda35
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082402"
---
# <a name="conditionalaccessfilter-resource-type"></a><span data-ttu-id="e2be4-103">Tipo de recurso conditionalAccessFilter</span><span class="sxs-lookup"><span data-stu-id="e2be4-103">conditionalAccessFilter resource type</span></span>

<span data-ttu-id="e2be4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2be4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2be4-105">Representa o filtro no escopo da política.</span><span class="sxs-lookup"><span data-stu-id="e2be4-105">Represents filter in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="e2be4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2be4-106">Properties</span></span>

| <span data-ttu-id="e2be4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2be4-107">Property</span></span>     | <span data-ttu-id="e2be4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2be4-108">Type</span></span>        | <span data-ttu-id="e2be4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2be4-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e2be4-110">modo</span><span class="sxs-lookup"><span data-stu-id="e2be4-110">mode</span></span> | <span data-ttu-id="e2be4-111">filterMode</span><span class="sxs-lookup"><span data-stu-id="e2be4-111">filterMode</span></span> | <span data-ttu-id="e2be4-112">Modo a ser usado para o filtro.</span><span class="sxs-lookup"><span data-stu-id="e2be4-112">Mode to use for the filter.</span></span> <span data-ttu-id="e2be4-113">Os valores possíveis são: `include` ou `exclude`.</span><span class="sxs-lookup"><span data-stu-id="e2be4-113">Possible values are `include` or `exclude`.</span></span> |
| <span data-ttu-id="e2be4-114">rule</span><span class="sxs-lookup"><span data-stu-id="e2be4-114">rule</span></span> | <span data-ttu-id="e2be4-115">String</span><span class="sxs-lookup"><span data-stu-id="e2be4-115">String</span></span> | <span data-ttu-id="e2be4-116">A sintaxe de regra é semelhante à usada para regras de associação para grupos no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e2be4-116">Rule syntax is similar to that used for membership rules for groups in Azure AD.</span></span> <span data-ttu-id="e2be4-117">Para obter detalhes, consulte [regras com várias expressões](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span><span class="sxs-lookup"><span data-stu-id="e2be4-117">For details, see [rules with multiple expressions](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2be4-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e2be4-118">Relationships</span></span>

<span data-ttu-id="e2be4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2be4-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2be4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2be4-120">JSON representation</span></span>

<span data-ttu-id="e2be4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2be4-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


