---
title: Tipo de recurso keyValuePair
description: Par de valores de chave para parâmetros de ação.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2417ada5a3fa3937d6560f62a47c99f6b47d44e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523013"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="3086b-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="3086b-103">keyValuePair resource type</span></span>

<span data-ttu-id="3086b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3086b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3086b-105">Par de valores de chave para parâmetros de ação.</span><span class="sxs-lookup"><span data-stu-id="3086b-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="3086b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3086b-106">Properties</span></span>

| <span data-ttu-id="3086b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3086b-107">Property</span></span>     | <span data-ttu-id="3086b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3086b-108">Type</span></span>        | <span data-ttu-id="3086b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3086b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3086b-110">nome</span><span class="sxs-lookup"><span data-stu-id="3086b-110">name</span></span>|<span data-ttu-id="3086b-111">String</span><span class="sxs-lookup"><span data-stu-id="3086b-111">String</span></span>|<span data-ttu-id="3086b-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="3086b-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="3086b-113">value</span><span class="sxs-lookup"><span data-stu-id="3086b-113">value</span></span>|<span data-ttu-id="3086b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3086b-114">String</span></span>|<span data-ttu-id="3086b-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="3086b-115">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3086b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3086b-116">JSON representation</span></span>

<span data-ttu-id="3086b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3086b-117">The following is a JSON representation of the resource.</span></span>

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