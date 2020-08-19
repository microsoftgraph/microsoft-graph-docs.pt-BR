---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a6ea27f1dd6206a97b6ad60daf783b3092b69a4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807021"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="062d8-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="062d8-103">patchContentCommand resource type</span></span>

<span data-ttu-id="062d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="062d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="062d8-105">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="062d8-105">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="062d8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="062d8-106">JSON representation</span></span>

<span data-ttu-id="062d8-107">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="062d8-107">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span>

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

## <a name="properties"></a><span data-ttu-id="062d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="062d8-108">Properties</span></span>
| <span data-ttu-id="062d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="062d8-109">Property</span></span>     | <span data-ttu-id="062d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="062d8-110">Type</span></span>   |<span data-ttu-id="062d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="062d8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="062d8-112">ação</span><span class="sxs-lookup"><span data-stu-id="062d8-112">action</span></span>|<span data-ttu-id="062d8-113">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="062d8-113">onenotePatchActionType</span></span>|<span data-ttu-id="062d8-114">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="062d8-114">The action to perform on the target element.</span></span> <span data-ttu-id="062d8-115">Os valores possíveis são: `replace` , `append` , `delete` , `insert` , ou `prepend` .</span><span class="sxs-lookup"><span data-stu-id="062d8-115">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="062d8-116">content</span><span class="sxs-lookup"><span data-stu-id="062d8-116">content</span></span>|<span data-ttu-id="062d8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="062d8-117">String</span></span>|<span data-ttu-id="062d8-118">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="062d8-118">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="062d8-119">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o `multipart/form-data` tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="062d8-119">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="062d8-120">position</span><span class="sxs-lookup"><span data-stu-id="062d8-120">position</span></span>|<span data-ttu-id="062d8-121">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="062d8-121">onenotePatchInsertPosition</span></span>|<span data-ttu-id="062d8-122">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="062d8-122">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="062d8-123">Os valores possíveis são: `after` (padrão) ou `before` .</span><span class="sxs-lookup"><span data-stu-id="062d8-123">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="062d8-124">destino</span><span class="sxs-lookup"><span data-stu-id="062d8-124">target</span></span>|<span data-ttu-id="062d8-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="062d8-125">String</span></span>|<span data-ttu-id="062d8-126">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="062d8-126">The element to update.</span></span> <span data-ttu-id="062d8-127">Deve ser o `#<data-id>` ou o gerado `<id>` do elemento, ou a `body` `title` palavra-chave ou.</span><span class="sxs-lookup"><span data-stu-id="062d8-127">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
