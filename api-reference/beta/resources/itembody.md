---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
ms.openlocfilehash: 4ceada2ffe8106c270aa262d32ff85e349a8e657
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033214"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="9d5a3-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="9d5a3-103">itemBody resource type</span></span>

> <span data-ttu-id="9d5a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d5a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d5a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d5a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d5a3-106">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="9d5a3-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="9d5a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d5a3-107">Properties</span></span>
| <span data-ttu-id="9d5a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d5a3-108">Property</span></span>     | <span data-ttu-id="9d5a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d5a3-109">Type</span></span>   |<span data-ttu-id="9d5a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d5a3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d5a3-111">content</span><span class="sxs-lookup"><span data-stu-id="9d5a3-111">content</span></span>|<span data-ttu-id="9d5a3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d5a3-112">String</span></span>|<span data-ttu-id="9d5a3-113">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="9d5a3-113">The content of the item.</span></span>|
|<span data-ttu-id="9d5a3-114">contentType</span><span class="sxs-lookup"><span data-stu-id="9d5a3-114">contentType</span></span>|<span data-ttu-id="9d5a3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d5a3-115">String</span></span>|<span data-ttu-id="9d5a3-p102">O tipo de conteúdo. Os valores possíveis são: `Text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="9d5a3-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d5a3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d5a3-118">JSON representation</span></span>

<span data-ttu-id="9d5a3-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9d5a3-119">Here is a JSON representation of the resource</span></span>

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
