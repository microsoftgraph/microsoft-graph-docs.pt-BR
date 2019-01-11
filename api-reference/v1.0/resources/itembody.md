---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: 2eaf3b5e13833665c452eeecd74169915f5ac2fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805226"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="c99e0-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="c99e0-103">itemBody resource type</span></span>

<span data-ttu-id="c99e0-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="c99e0-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="c99e0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c99e0-105">Properties</span></span>
| <span data-ttu-id="c99e0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c99e0-106">Property</span></span>     | <span data-ttu-id="c99e0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c99e0-107">Type</span></span>   |<span data-ttu-id="c99e0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c99e0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c99e0-109">content</span><span class="sxs-lookup"><span data-stu-id="c99e0-109">content</span></span>|<span data-ttu-id="c99e0-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c99e0-110">String</span></span>|<span data-ttu-id="c99e0-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c99e0-111">The content of the item.</span></span>|
|<span data-ttu-id="c99e0-112">contentType</span><span class="sxs-lookup"><span data-stu-id="c99e0-112">contentType</span></span>|<span data-ttu-id="c99e0-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="c99e0-113">bodyType</span></span>|<span data-ttu-id="c99e0-p101">O tipo de conteúdo. Os valores possíveis são: `Text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="c99e0-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c99e0-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c99e0-116">JSON representation</span></span>

<span data-ttu-id="c99e0-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c99e0-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
