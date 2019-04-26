---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
ms.openlocfilehash: 66b4438b73f0000c172db1df385088528d221be4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324798"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="17325-104">tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="17325-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17325-105">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="17325-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="17325-106">Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="17325-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="17325-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17325-107">Properties</span></span>
| <span data-ttu-id="17325-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17325-108">Property</span></span>     | <span data-ttu-id="17325-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="17325-109">Type</span></span>   |<span data-ttu-id="17325-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="17325-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17325-111">key</span><span class="sxs-lookup"><span data-stu-id="17325-111">key</span></span>|<span data-ttu-id="17325-112">String</span><span class="sxs-lookup"><span data-stu-id="17325-112">String</span></span>|<span data-ttu-id="17325-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="17325-113">Key.</span></span>|
|<span data-ttu-id="17325-114">valor</span><span class="sxs-lookup"><span data-stu-id="17325-114">value</span></span>|<span data-ttu-id="17325-115">Json</span><span class="sxs-lookup"><span data-stu-id="17325-115">Json</span></span>|<span data-ttu-id="17325-116">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="17325-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17325-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17325-117">JSON representation</span></span>

<span data-ttu-id="17325-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17325-118">The following is a JSON representation of the resource.</span></span>

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
