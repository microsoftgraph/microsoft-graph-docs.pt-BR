---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b97f1f8bf10005a9e7829ee9280ebf936405b346
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620624"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="c1029-104">tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="c1029-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1029-105">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="c1029-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="c1029-106">Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="c1029-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="c1029-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1029-107">Properties</span></span>
| <span data-ttu-id="c1029-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1029-108">Property</span></span>     | <span data-ttu-id="c1029-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1029-109">Type</span></span>   |<span data-ttu-id="c1029-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1029-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1029-111">key</span><span class="sxs-lookup"><span data-stu-id="c1029-111">key</span></span>|<span data-ttu-id="c1029-112">String</span><span class="sxs-lookup"><span data-stu-id="c1029-112">String</span></span>|<span data-ttu-id="c1029-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="c1029-113">Key.</span></span>|
|<span data-ttu-id="c1029-114">valor</span><span class="sxs-lookup"><span data-stu-id="c1029-114">value</span></span>|<span data-ttu-id="c1029-115">Json</span><span class="sxs-lookup"><span data-stu-id="c1029-115">Json</span></span>|<span data-ttu-id="c1029-116">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="c1029-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1029-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1029-117">JSON representation</span></span>

<span data-ttu-id="c1029-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1029-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
