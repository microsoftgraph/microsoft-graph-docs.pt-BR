---
title: Tipo de recurso keyValuePair
description: Par de valores de chave para parâmetros de ação.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366935"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="263b2-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="263b2-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="263b2-104">Par de valores de chave para parâmetros de ação.</span><span class="sxs-lookup"><span data-stu-id="263b2-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="263b2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="263b2-105">Properties</span></span>

| <span data-ttu-id="263b2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="263b2-106">Property</span></span>     | <span data-ttu-id="263b2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="263b2-107">Type</span></span>        | <span data-ttu-id="263b2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="263b2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="263b2-109">name</span><span class="sxs-lookup"><span data-stu-id="263b2-109">name</span></span>|<span data-ttu-id="263b2-110">String</span><span class="sxs-lookup"><span data-stu-id="263b2-110">String</span></span>|<span data-ttu-id="263b2-111">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="263b2-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="263b2-112">valor</span><span class="sxs-lookup"><span data-stu-id="263b2-112">value</span></span>|<span data-ttu-id="263b2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="263b2-113">String</span></span>|<span data-ttu-id="263b2-114">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="263b2-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="263b2-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="263b2-115">JSON representation</span></span>

<span data-ttu-id="263b2-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="263b2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->