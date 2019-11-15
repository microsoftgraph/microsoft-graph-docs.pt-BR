---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 0bba7fce9557c6c249ea9aefced5a198a87f5026
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658804"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="fee28-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="fee28-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee28-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="fee28-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="fee28-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fee28-105">Properties</span></span>
| <span data-ttu-id="fee28-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fee28-106">Property</span></span>     | <span data-ttu-id="fee28-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee28-107">Type</span></span>   |<span data-ttu-id="fee28-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee28-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fee28-109">content</span><span class="sxs-lookup"><span data-stu-id="fee28-109">content</span></span>|<span data-ttu-id="fee28-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fee28-110">String</span></span>|<span data-ttu-id="fee28-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="fee28-111">The content of the item.</span></span>|
|<span data-ttu-id="fee28-112">contentType</span><span class="sxs-lookup"><span data-stu-id="fee28-112">contentType</span></span>|<span data-ttu-id="fee28-113">String</span><span class="sxs-lookup"><span data-stu-id="fee28-113">String</span></span>|<span data-ttu-id="fee28-p101">O tipo de conteúdo. Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="fee28-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fee28-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fee28-116">JSON representation</span></span>

<span data-ttu-id="fee28-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fee28-117">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
