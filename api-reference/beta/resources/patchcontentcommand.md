---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568464"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="64a55-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="64a55-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a55-104">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="64a55-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64a55-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64a55-105">JSON representation</span></span>

<span data-ttu-id="64a55-106">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="64a55-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="64a55-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64a55-107">Properties</span></span>
| <span data-ttu-id="64a55-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64a55-108">Property</span></span>     | <span data-ttu-id="64a55-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="64a55-109">Type</span></span>   |<span data-ttu-id="64a55-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="64a55-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64a55-111">ação</span><span class="sxs-lookup"><span data-stu-id="64a55-111">action</span></span>|<span data-ttu-id="64a55-112">String</span><span class="sxs-lookup"><span data-stu-id="64a55-112">String</span></span>|<span data-ttu-id="64a55-113">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="64a55-113">The action to perform on the target element.</span></span> <span data-ttu-id="64a55-114">Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="64a55-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="64a55-115">content</span><span class="sxs-lookup"><span data-stu-id="64a55-115">content</span></span>|<span data-ttu-id="64a55-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64a55-116">String</span></span>|<span data-ttu-id="64a55-117">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="64a55-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="64a55-118">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="64a55-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="64a55-119">position</span><span class="sxs-lookup"><span data-stu-id="64a55-119">position</span></span>|<span data-ttu-id="64a55-120">String</span><span class="sxs-lookup"><span data-stu-id="64a55-120">String</span></span>|<span data-ttu-id="64a55-121">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="64a55-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="64a55-122">Os valores possíveis são `after` : (padrão) `before`ou.</span><span class="sxs-lookup"><span data-stu-id="64a55-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="64a55-123">destino</span><span class="sxs-lookup"><span data-stu-id="64a55-123">target</span></span>|<span data-ttu-id="64a55-124">String</span><span class="sxs-lookup"><span data-stu-id="64a55-124">String</span></span>|<span data-ttu-id="64a55-125">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="64a55-125">The element to update.</span></span> <span data-ttu-id="64a55-126">Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="64a55-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

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
