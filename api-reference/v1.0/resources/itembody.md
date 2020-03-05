---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fb7fea89a7da3d98899a19614d7c40f76dcb6f8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447644"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="597f3-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="597f3-103">itemBody resource type</span></span>

<span data-ttu-id="597f3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="597f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="597f3-105">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="597f3-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="597f3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="597f3-106">Properties</span></span>
| <span data-ttu-id="597f3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="597f3-107">Property</span></span>     | <span data-ttu-id="597f3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="597f3-108">Type</span></span>   |<span data-ttu-id="597f3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="597f3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="597f3-110">content</span><span class="sxs-lookup"><span data-stu-id="597f3-110">content</span></span>|<span data-ttu-id="597f3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="597f3-111">String</span></span>|<span data-ttu-id="597f3-112">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="597f3-112">The content of the item.</span></span>|
|<span data-ttu-id="597f3-113">contentType</span><span class="sxs-lookup"><span data-stu-id="597f3-113">contentType</span></span>|<span data-ttu-id="597f3-114">BodyType</span><span class="sxs-lookup"><span data-stu-id="597f3-114">bodyType</span></span>|<span data-ttu-id="597f3-115">O tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="597f3-115">The type of the content.</span></span> <span data-ttu-id="597f3-116">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="597f3-116">Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="597f3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="597f3-117">JSON representation</span></span>

<span data-ttu-id="597f3-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="597f3-118">Here is a JSON representation of the resource</span></span>

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
