---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585304"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="a0404-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="a0404-103">itemBody resource type</span></span>

<span data-ttu-id="a0404-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="a0404-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="a0404-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0404-105">Properties</span></span>
| <span data-ttu-id="a0404-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0404-106">Property</span></span>     | <span data-ttu-id="a0404-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0404-107">Type</span></span>   |<span data-ttu-id="a0404-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0404-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0404-109">content</span><span class="sxs-lookup"><span data-stu-id="a0404-109">content</span></span>|<span data-ttu-id="a0404-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0404-110">String</span></span>|<span data-ttu-id="a0404-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="a0404-111">The content of the item.</span></span>|
|<span data-ttu-id="a0404-112">contentType</span><span class="sxs-lookup"><span data-stu-id="a0404-112">contentType</span></span>|<span data-ttu-id="a0404-113">BodyType</span><span class="sxs-lookup"><span data-stu-id="a0404-113">bodyType</span></span>|<span data-ttu-id="a0404-114">O tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a0404-114">The type of the content.</span></span> <span data-ttu-id="a0404-115">Os valores possíveis são: `text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="a0404-115">Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0404-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0404-116">JSON representation</span></span>

<span data-ttu-id="a0404-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a0404-117">Here is a JSON representation of the resource</span></span>

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
