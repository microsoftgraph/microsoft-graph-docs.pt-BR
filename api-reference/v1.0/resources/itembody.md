---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 406a753ef8b58ba5ff19f7669239c3d9abb860c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036551"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="265af-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="265af-103">itemBody resource type</span></span>

<span data-ttu-id="265af-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="265af-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="265af-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="265af-105">Properties</span></span>
| <span data-ttu-id="265af-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="265af-106">Property</span></span>     | <span data-ttu-id="265af-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="265af-107">Type</span></span>   |<span data-ttu-id="265af-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="265af-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="265af-109">content</span><span class="sxs-lookup"><span data-stu-id="265af-109">content</span></span>|<span data-ttu-id="265af-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="265af-110">String</span></span>|<span data-ttu-id="265af-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="265af-111">The content of the item.</span></span>|
|<span data-ttu-id="265af-112">contentType</span><span class="sxs-lookup"><span data-stu-id="265af-112">contentType</span></span>|<span data-ttu-id="265af-113">BodyType</span><span class="sxs-lookup"><span data-stu-id="265af-113">bodyType</span></span>|<span data-ttu-id="265af-114">O tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="265af-114">The type of the content.</span></span> <span data-ttu-id="265af-115">Os valores possíveis são: `text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="265af-115">Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="265af-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="265af-116">JSON representation</span></span>

<span data-ttu-id="265af-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="265af-117">Here is a JSON representation of the resource</span></span>

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
