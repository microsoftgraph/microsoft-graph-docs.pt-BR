---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3a86cd4963f8d17fbe9f4c5371e98070f8f8f4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520090"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="a3b70-104">tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="a3b70-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="a3b70-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3b70-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3b70-106">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="a3b70-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="a3b70-107">Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="a3b70-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="a3b70-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3b70-108">Properties</span></span>
| <span data-ttu-id="a3b70-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3b70-109">Property</span></span>     | <span data-ttu-id="a3b70-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3b70-110">Type</span></span>   |<span data-ttu-id="a3b70-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3b70-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3b70-112">key</span><span class="sxs-lookup"><span data-stu-id="a3b70-112">key</span></span>|<span data-ttu-id="a3b70-113">String</span><span class="sxs-lookup"><span data-stu-id="a3b70-113">String</span></span>|<span data-ttu-id="a3b70-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="a3b70-114">Key.</span></span>|
|<span data-ttu-id="a3b70-115">valor</span><span class="sxs-lookup"><span data-stu-id="a3b70-115">value</span></span>|<span data-ttu-id="a3b70-116">Json</span><span class="sxs-lookup"><span data-stu-id="a3b70-116">Json</span></span>|<span data-ttu-id="a3b70-117">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="a3b70-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3b70-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3b70-118">JSON representation</span></span>

<span data-ttu-id="a3b70-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3b70-119">The following is a JSON representation of the resource.</span></span>

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
