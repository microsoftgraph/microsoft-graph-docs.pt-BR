---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
ms.openlocfilehash: 80fa4308fdcf5dc05287051f6ae586b228a02073
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344972"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="df457-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="df457-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df457-104">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="df457-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df457-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df457-105">JSON representation</span></span>

<span data-ttu-id="df457-106">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="df457-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="df457-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df457-107">Properties</span></span>
| <span data-ttu-id="df457-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df457-108">Property</span></span>     | <span data-ttu-id="df457-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df457-109">Type</span></span>   |<span data-ttu-id="df457-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df457-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df457-111">ação</span><span class="sxs-lookup"><span data-stu-id="df457-111">action</span></span>|<span data-ttu-id="df457-112">String</span><span class="sxs-lookup"><span data-stu-id="df457-112">String</span></span>|<span data-ttu-id="df457-113">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="df457-113">The action to perform on the target element.</span></span> <span data-ttu-id="df457-114">Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="df457-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="df457-115">content</span><span class="sxs-lookup"><span data-stu-id="df457-115">content</span></span>|<span data-ttu-id="df457-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df457-116">String</span></span>|<span data-ttu-id="df457-117">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="df457-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="df457-118">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="df457-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="df457-119">position</span><span class="sxs-lookup"><span data-stu-id="df457-119">position</span></span>|<span data-ttu-id="df457-120">String</span><span class="sxs-lookup"><span data-stu-id="df457-120">String</span></span>|<span data-ttu-id="df457-121">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="df457-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="df457-122">Os valores possíveis são `after` : (padrão) `before`ou.</span><span class="sxs-lookup"><span data-stu-id="df457-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="df457-123">destino</span><span class="sxs-lookup"><span data-stu-id="df457-123">target</span></span>|<span data-ttu-id="df457-124">String</span><span class="sxs-lookup"><span data-stu-id="df457-124">String</span></span>|<span data-ttu-id="df457-125">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="df457-125">The element to update.</span></span> <span data-ttu-id="df457-126">Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="df457-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

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
