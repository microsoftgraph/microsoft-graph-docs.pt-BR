---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
ms.openlocfilehash: ebcc2797052ac3a5a73547332e37c5e9c1bd3a41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006082"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="1b939-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="1b939-103">itemBody resource type</span></span>

<span data-ttu-id="1b939-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="1b939-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="1b939-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b939-105">Properties</span></span>
| <span data-ttu-id="1b939-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b939-106">Property</span></span>     | <span data-ttu-id="1b939-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b939-107">Type</span></span>   |<span data-ttu-id="1b939-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b939-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b939-109">content</span><span class="sxs-lookup"><span data-stu-id="1b939-109">content</span></span>|<span data-ttu-id="1b939-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b939-110">String</span></span>|<span data-ttu-id="1b939-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="1b939-111">The content of the item.</span></span>|
|<span data-ttu-id="1b939-112">contentType</span><span class="sxs-lookup"><span data-stu-id="1b939-112">contentType</span></span>|<span data-ttu-id="1b939-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="1b939-113">bodyType</span></span>|<span data-ttu-id="1b939-p101">O tipo de conteúdo. Os valores possíveis são: `Text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="1b939-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b939-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b939-116">JSON representation</span></span>

<span data-ttu-id="1b939-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1b939-117">Here is a JSON representation of the resource</span></span>

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
