---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: 1cf79f78caa7b2772bc44b99c6b9bdc526340a87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523472"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="0fa65-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="0fa65-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fa65-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="0fa65-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="0fa65-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0fa65-105">Properties</span></span>
| <span data-ttu-id="0fa65-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0fa65-106">Property</span></span>     | <span data-ttu-id="0fa65-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0fa65-107">Type</span></span>   |<span data-ttu-id="0fa65-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0fa65-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fa65-109">content</span><span class="sxs-lookup"><span data-stu-id="0fa65-109">content</span></span>|<span data-ttu-id="0fa65-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0fa65-110">String</span></span>|<span data-ttu-id="0fa65-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="0fa65-111">The content of the item.</span></span>|
|<span data-ttu-id="0fa65-112">contentType</span><span class="sxs-lookup"><span data-stu-id="0fa65-112">contentType</span></span>|<span data-ttu-id="0fa65-113">String</span><span class="sxs-lookup"><span data-stu-id="0fa65-113">String</span></span>|<span data-ttu-id="0fa65-p101">O tipo de conteúdo. Os valores possíveis são: `text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="0fa65-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fa65-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0fa65-116">JSON representation</span></span>

<span data-ttu-id="0fa65-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0fa65-117">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
