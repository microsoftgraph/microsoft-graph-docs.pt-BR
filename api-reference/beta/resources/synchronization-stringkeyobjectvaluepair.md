---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2b7c32a0048e3aafa3c0c56ff91f1ae51542914
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026135"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="e914c-104">tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="e914c-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="e914c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e914c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e914c-106">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="e914c-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="e914c-107">Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="e914c-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="e914c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e914c-108">Properties</span></span>
| <span data-ttu-id="e914c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e914c-109">Property</span></span>     | <span data-ttu-id="e914c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e914c-110">Type</span></span>   |<span data-ttu-id="e914c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e914c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e914c-112">key</span><span class="sxs-lookup"><span data-stu-id="e914c-112">key</span></span>|<span data-ttu-id="e914c-113">String</span><span class="sxs-lookup"><span data-stu-id="e914c-113">String</span></span>|<span data-ttu-id="e914c-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="e914c-114">Key.</span></span>|
|<span data-ttu-id="e914c-115">valor</span><span class="sxs-lookup"><span data-stu-id="e914c-115">value</span></span>|<span data-ttu-id="e914c-116">Json</span><span class="sxs-lookup"><span data-stu-id="e914c-116">Json</span></span>|<span data-ttu-id="e914c-117">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="e914c-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e914c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e914c-118">JSON representation</span></span>

<span data-ttu-id="e914c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e914c-119">The following is a JSON representation of the resource.</span></span>

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


