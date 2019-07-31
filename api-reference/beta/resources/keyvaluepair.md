---
title: Tipo de recurso keyValuePair
description: Par de valores de chave para parâmetros de ação.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db8d3b14ceaa0ff05181894af803b8b6feea77c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967032"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="1648c-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="1648c-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1648c-104">Par de valores de chave para parâmetros de ação.</span><span class="sxs-lookup"><span data-stu-id="1648c-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="1648c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1648c-105">Properties</span></span>

| <span data-ttu-id="1648c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1648c-106">Property</span></span>     | <span data-ttu-id="1648c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1648c-107">Type</span></span>        | <span data-ttu-id="1648c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1648c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1648c-109">name</span><span class="sxs-lookup"><span data-stu-id="1648c-109">name</span></span>|<span data-ttu-id="1648c-110">String</span><span class="sxs-lookup"><span data-stu-id="1648c-110">String</span></span>|<span data-ttu-id="1648c-111">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="1648c-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="1648c-112">value</span><span class="sxs-lookup"><span data-stu-id="1648c-112">value</span></span>|<span data-ttu-id="1648c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1648c-113">String</span></span>|<span data-ttu-id="1648c-114">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="1648c-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1648c-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1648c-115">JSON representation</span></span>

<span data-ttu-id="1648c-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1648c-116">The following is a JSON representation of the resource.</span></span>

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