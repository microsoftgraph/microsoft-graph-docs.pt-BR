---
title: tipo de recurso de stringKeyObjectValuePair
description: Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.
localization_priority: Normal
ms.openlocfilehash: 819a2e004ee712f1250652ce0b3811940545e643
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572168"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="df970-104">tipo de recurso de stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="df970-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df970-105">Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="df970-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="df970-106">Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="df970-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="df970-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df970-107">Properties</span></span>
| <span data-ttu-id="df970-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df970-108">Property</span></span>     | <span data-ttu-id="df970-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df970-109">Type</span></span>   |<span data-ttu-id="df970-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df970-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df970-111">key</span><span class="sxs-lookup"><span data-stu-id="df970-111">key</span></span>|<span data-ttu-id="df970-112">String</span><span class="sxs-lookup"><span data-stu-id="df970-112">String</span></span>|<span data-ttu-id="df970-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="df970-113">Key.</span></span>|
|<span data-ttu-id="df970-114">valor</span><span class="sxs-lookup"><span data-stu-id="df970-114">value</span></span>|<span data-ttu-id="df970-115">Json</span><span class="sxs-lookup"><span data-stu-id="df970-115">Json</span></span>|<span data-ttu-id="df970-116">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="df970-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df970-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df970-117">JSON representation</span></span>

<span data-ttu-id="df970-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df970-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value":"Json"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-stringkeyobjectvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
