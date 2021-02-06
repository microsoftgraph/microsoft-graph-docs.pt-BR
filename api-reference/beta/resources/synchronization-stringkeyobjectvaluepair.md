---
title: Tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Esse é um tipo aberto OData que espera ter uma propriedade chamada `value` que é um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 535e9f104f42771e6f6c182769f0a5e1f68169b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137062"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="d69c9-104">Tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="d69c9-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="d69c9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d69c9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d69c9-106">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="d69c9-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="d69c9-107">Esse é um tipo aberto OData que espera ter uma propriedade chamada `value` que é um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="d69c9-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="d69c9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d69c9-108">Properties</span></span>
| <span data-ttu-id="d69c9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d69c9-109">Property</span></span>     | <span data-ttu-id="d69c9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d69c9-110">Type</span></span>   |<span data-ttu-id="d69c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d69c9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d69c9-112">key</span><span class="sxs-lookup"><span data-stu-id="d69c9-112">key</span></span>|<span data-ttu-id="d69c9-113">String</span><span class="sxs-lookup"><span data-stu-id="d69c9-113">String</span></span>|<span data-ttu-id="d69c9-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="d69c9-114">Key.</span></span>|
|<span data-ttu-id="d69c9-115">valor</span><span class="sxs-lookup"><span data-stu-id="d69c9-115">value</span></span>|<span data-ttu-id="d69c9-116">Json</span><span class="sxs-lookup"><span data-stu-id="d69c9-116">Json</span></span>|<span data-ttu-id="d69c9-117">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="d69c9-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d69c9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d69c9-118">JSON representation</span></span>

<span data-ttu-id="d69c9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d69c9-119">The following is a JSON representation of the resource.</span></span>

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


