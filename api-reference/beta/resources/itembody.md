---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 8ee076b96df14b4d4c4958b4c1d6bdf36fecdde2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075613"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="5e78c-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="5e78c-103">itemBody resource type</span></span>

<span data-ttu-id="5e78c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e78c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e78c-105">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="5e78c-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="5e78c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e78c-106">Properties</span></span>
| <span data-ttu-id="5e78c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e78c-107">Property</span></span>     | <span data-ttu-id="5e78c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e78c-108">Type</span></span>   |<span data-ttu-id="5e78c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e78c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e78c-110">content</span><span class="sxs-lookup"><span data-stu-id="5e78c-110">content</span></span>|<span data-ttu-id="5e78c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e78c-111">String</span></span>|<span data-ttu-id="5e78c-112">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="5e78c-112">The content of the item.</span></span>|
|<span data-ttu-id="5e78c-113">contentType</span><span class="sxs-lookup"><span data-stu-id="5e78c-113">contentType</span></span>|<span data-ttu-id="5e78c-114">String</span><span class="sxs-lookup"><span data-stu-id="5e78c-114">String</span></span>|<span data-ttu-id="5e78c-p101">O tipo de conteúdo. Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="5e78c-p101">The type of the content. Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e78c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e78c-117">JSON representation</span></span>

<span data-ttu-id="5e78c-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5e78c-118">Here is a JSON representation of the resource</span></span>

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


