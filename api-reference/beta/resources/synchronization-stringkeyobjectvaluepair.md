---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a04df77ee010368b73abfe5a2d8d78cfe99b0b4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217560"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="4ae0c-104">tipo de recurso stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="4ae0c-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="4ae0c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ae0c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae0c-106">Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="4ae0c-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="4ae0c-107">Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="4ae0c-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="4ae0c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ae0c-108">Properties</span></span>
| <span data-ttu-id="4ae0c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ae0c-109">Property</span></span>     | <span data-ttu-id="4ae0c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ae0c-110">Type</span></span>   |<span data-ttu-id="4ae0c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ae0c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ae0c-112">key</span><span class="sxs-lookup"><span data-stu-id="4ae0c-112">key</span></span>|<span data-ttu-id="4ae0c-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4ae0c-113">String</span></span>|<span data-ttu-id="4ae0c-114">Chave.</span><span class="sxs-lookup"><span data-stu-id="4ae0c-114">Key.</span></span>|
|<span data-ttu-id="4ae0c-115">valor</span><span class="sxs-lookup"><span data-stu-id="4ae0c-115">value</span></span>|<span data-ttu-id="4ae0c-116">Json</span><span class="sxs-lookup"><span data-stu-id="4ae0c-116">Json</span></span>|<span data-ttu-id="4ae0c-117">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="4ae0c-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ae0c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ae0c-118">JSON representation</span></span>

<span data-ttu-id="4ae0c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ae0c-119">The following is a JSON representation of the resource.</span></span>

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
