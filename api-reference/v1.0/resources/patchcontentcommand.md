---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3c8aab8770304f8616025d0d5ac2e70ad41a1340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534075"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="d966d-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="d966d-103">patchContentCommand resource type</span></span>

<span data-ttu-id="d966d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d966d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d966d-105">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="d966d-105">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d966d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d966d-106">JSON representation</span></span>

<span data-ttu-id="d966d-107">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="d966d-107">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="d966d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d966d-108">Properties</span></span>
| <span data-ttu-id="d966d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d966d-109">Property</span></span>     | <span data-ttu-id="d966d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d966d-110">Type</span></span>   |<span data-ttu-id="d966d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d966d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d966d-112">ação</span><span class="sxs-lookup"><span data-stu-id="d966d-112">action</span></span>|<span data-ttu-id="d966d-113">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="d966d-113">onenotePatchActionType</span></span>|<span data-ttu-id="d966d-114">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="d966d-114">The action to perform on the target element.</span></span> <span data-ttu-id="d966d-115">Os valores possíveis são: `replace`, `append`, `delete`, `insert`, ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="d966d-115">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="d966d-116">content</span><span class="sxs-lookup"><span data-stu-id="d966d-116">content</span></span>|<span data-ttu-id="d966d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d966d-117">String</span></span>|<span data-ttu-id="d966d-118">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="d966d-118">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="d966d-119">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="d966d-119">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="d966d-120">position</span><span class="sxs-lookup"><span data-stu-id="d966d-120">position</span></span>|<span data-ttu-id="d966d-121">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="d966d-121">onenotePatchInsertPosition</span></span>|<span data-ttu-id="d966d-122">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="d966d-122">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="d966d-123">Os valores possíveis são: `after` (padrão) ou `before`.</span><span class="sxs-lookup"><span data-stu-id="d966d-123">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="d966d-124">destino</span><span class="sxs-lookup"><span data-stu-id="d966d-124">target</span></span>|<span data-ttu-id="d966d-125">String</span><span class="sxs-lookup"><span data-stu-id="d966d-125">String</span></span>|<span data-ttu-id="d966d-126">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d966d-126">The element to update.</span></span> <span data-ttu-id="d966d-127">Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="d966d-127">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
