---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 21f2be43bc31d7611cf43ebd228850e3993807fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952782"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="73a7e-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="73a7e-103">itemBody resource type</span></span>

<span data-ttu-id="73a7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73a7e-105">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="73a7e-105">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="73a7e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73a7e-106">Properties</span></span>
| <span data-ttu-id="73a7e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73a7e-107">Property</span></span>     | <span data-ttu-id="73a7e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="73a7e-108">Type</span></span>   |<span data-ttu-id="73a7e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a7e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73a7e-110">content</span><span class="sxs-lookup"><span data-stu-id="73a7e-110">content</span></span>|<span data-ttu-id="73a7e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73a7e-111">String</span></span>|<span data-ttu-id="73a7e-112">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="73a7e-112">The content of the item.</span></span>|
|<span data-ttu-id="73a7e-113">contentType</span><span class="sxs-lookup"><span data-stu-id="73a7e-113">contentType</span></span>|<span data-ttu-id="73a7e-114">bodyType</span><span class="sxs-lookup"><span data-stu-id="73a7e-114">bodyType</span></span>|<span data-ttu-id="73a7e-115">O tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="73a7e-115">The type of the content.</span></span> <span data-ttu-id="73a7e-116">Os valores possíveis são: `text` e `html`.</span><span class="sxs-lookup"><span data-stu-id="73a7e-116">Possible values are `text` and `html`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73a7e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73a7e-117">JSON representation</span></span>

<span data-ttu-id="73a7e-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="73a7e-118">Here is a JSON representation of the resource</span></span>

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


