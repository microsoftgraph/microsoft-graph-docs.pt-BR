---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462540"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="75278-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="75278-103">patchContentCommand resource type</span></span>

<span data-ttu-id="75278-104">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="75278-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75278-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75278-105">JSON representation</span></span>

<span data-ttu-id="75278-106">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="75278-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="75278-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75278-107">Properties</span></span>
| <span data-ttu-id="75278-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75278-108">Property</span></span>     | <span data-ttu-id="75278-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="75278-109">Type</span></span>   |<span data-ttu-id="75278-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75278-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75278-111">ação</span><span class="sxs-lookup"><span data-stu-id="75278-111">action</span></span>|<span data-ttu-id="75278-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="75278-112">onenotePatchActionType</span></span>|<span data-ttu-id="75278-113">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="75278-113">The action to perform on the target element.</span></span> <span data-ttu-id="75278-114">Os valores possíveis são: `replace`, `append`, `delete`, `insert`, ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="75278-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="75278-115">content</span><span class="sxs-lookup"><span data-stu-id="75278-115">content</span></span>|<span data-ttu-id="75278-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75278-116">String</span></span>|<span data-ttu-id="75278-117">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="75278-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="75278-118">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="75278-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="75278-119">position</span><span class="sxs-lookup"><span data-stu-id="75278-119">position</span></span>|<span data-ttu-id="75278-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="75278-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="75278-121">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="75278-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="75278-122">Os valores possíveis são: `after` (padrão) ou `before`.</span><span class="sxs-lookup"><span data-stu-id="75278-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="75278-123">destino</span><span class="sxs-lookup"><span data-stu-id="75278-123">target</span></span>|<span data-ttu-id="75278-124">String</span><span class="sxs-lookup"><span data-stu-id="75278-124">String</span></span>|<span data-ttu-id="75278-125">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="75278-125">The element to update.</span></span> <span data-ttu-id="75278-126">Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="75278-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
