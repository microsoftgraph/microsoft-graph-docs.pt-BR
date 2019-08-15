---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4cfa6fe84c18d4895e5d709d3ab6254258c1b970
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422279"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="10e76-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="10e76-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10e76-104">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="10e76-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10e76-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10e76-105">JSON representation</span></span>

<span data-ttu-id="10e76-106">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="10e76-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="10e76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10e76-107">Properties</span></span>
| <span data-ttu-id="10e76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10e76-108">Property</span></span>     | <span data-ttu-id="10e76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10e76-109">Type</span></span>   |<span data-ttu-id="10e76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10e76-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10e76-111">ação</span><span class="sxs-lookup"><span data-stu-id="10e76-111">action</span></span>|<span data-ttu-id="10e76-112">String</span><span class="sxs-lookup"><span data-stu-id="10e76-112">String</span></span>|<span data-ttu-id="10e76-113">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="10e76-113">The action to perform on the target element.</span></span> <span data-ttu-id="10e76-114">Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="10e76-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="10e76-115">content</span><span class="sxs-lookup"><span data-stu-id="10e76-115">content</span></span>|<span data-ttu-id="10e76-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10e76-116">String</span></span>|<span data-ttu-id="10e76-117">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="10e76-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="10e76-118">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="10e76-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="10e76-119">position</span><span class="sxs-lookup"><span data-stu-id="10e76-119">position</span></span>|<span data-ttu-id="10e76-120">String</span><span class="sxs-lookup"><span data-stu-id="10e76-120">String</span></span>|<span data-ttu-id="10e76-121">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="10e76-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="10e76-122">Os valores possíveis são `after` : (padrão) `before`ou.</span><span class="sxs-lookup"><span data-stu-id="10e76-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="10e76-123">destino</span><span class="sxs-lookup"><span data-stu-id="10e76-123">target</span></span>|<span data-ttu-id="10e76-124">String</span><span class="sxs-lookup"><span data-stu-id="10e76-124">String</span></span>|<span data-ttu-id="10e76-125">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="10e76-125">The element to update.</span></span> <span data-ttu-id="10e76-126">Deve ser o `#<data-id>` ou o gerado `{id}` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="10e76-126">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
