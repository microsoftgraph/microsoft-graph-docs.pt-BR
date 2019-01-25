---
title: Tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523880"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="1f57d-103">Tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="1f57d-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f57d-104">As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="1f57d-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f57d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f57d-105">JSON representation</span></span>

<span data-ttu-id="1f57d-106">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="1f57d-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="1f57d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f57d-107">Properties</span></span>
| <span data-ttu-id="1f57d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f57d-108">Property</span></span>     | <span data-ttu-id="1f57d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f57d-109">Type</span></span>   |<span data-ttu-id="1f57d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f57d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f57d-111">ação</span><span class="sxs-lookup"><span data-stu-id="1f57d-111">action</span></span>|<span data-ttu-id="1f57d-112">String</span><span class="sxs-lookup"><span data-stu-id="1f57d-112">String</span></span>|<span data-ttu-id="1f57d-p101">A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="1f57d-p101">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="1f57d-115">content</span><span class="sxs-lookup"><span data-stu-id="1f57d-115">content</span></span>|<span data-ttu-id="1f57d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f57d-116">String</span></span>|<span data-ttu-id="1f57d-p102">Uma cadeia de caracteres de HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="1f57d-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="1f57d-119">position</span><span class="sxs-lookup"><span data-stu-id="1f57d-119">position</span></span>|<span data-ttu-id="1f57d-120">String</span><span class="sxs-lookup"><span data-stu-id="1f57d-120">String</span></span>|<span data-ttu-id="1f57d-p103">O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before`.</span><span class="sxs-lookup"><span data-stu-id="1f57d-p103">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="1f57d-123">destino</span><span class="sxs-lookup"><span data-stu-id="1f57d-123">target</span></span>|<span data-ttu-id="1f57d-124">String</span><span class="sxs-lookup"><span data-stu-id="1f57d-124">String</span></span>|<span data-ttu-id="1f57d-p104">O elemento a atualizar. Deve ser `#<data-id>` ou o `<id>` gerado do elemento ou o `body` ou a palavra-chave de `title`.</span><span class="sxs-lookup"><span data-stu-id="1f57d-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
