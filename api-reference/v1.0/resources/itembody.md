---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6cf87c803ec957b42cc55cf1523a708b145af117
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657485"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="d39e6-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="d39e6-103">itemBody resource type</span></span>

<span data-ttu-id="d39e6-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="d39e6-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="d39e6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d39e6-105">Properties</span></span>
| <span data-ttu-id="d39e6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d39e6-106">Property</span></span>     | <span data-ttu-id="d39e6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d39e6-107">Type</span></span>   |<span data-ttu-id="d39e6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d39e6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d39e6-109">content</span><span class="sxs-lookup"><span data-stu-id="d39e6-109">content</span></span>|<span data-ttu-id="d39e6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d39e6-110">String</span></span>|<span data-ttu-id="d39e6-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="d39e6-111">The content of the item.</span></span>|
|<span data-ttu-id="d39e6-112">contentType</span><span class="sxs-lookup"><span data-stu-id="d39e6-112">contentType</span></span>|<span data-ttu-id="d39e6-113">BodyType</span><span class="sxs-lookup"><span data-stu-id="d39e6-113">bodyType</span></span>|<span data-ttu-id="d39e6-114">O tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d39e6-114">The type of the content.</span></span> <span data-ttu-id="d39e6-115">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="d39e6-115">Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d39e6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d39e6-116">JSON representation</span></span>

<span data-ttu-id="d39e6-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d39e6-117">Here is a JSON representation of the resource</span></span>

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
