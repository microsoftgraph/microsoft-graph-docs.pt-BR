---
title: tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f0b1ff2e4d8b6c312cf0a3a5be0acf70835fd788
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521994"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="31f74-103">tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="31f74-103">patchContentCommand resource type</span></span>

<span data-ttu-id="31f74-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31f74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31f74-105">As alterações a serem feitas em uma página do OneNote em uma solicitação de PATCH.</span><span class="sxs-lookup"><span data-stu-id="31f74-105">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31f74-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31f74-106">JSON representation</span></span>

<span data-ttu-id="31f74-107">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [patch Pages/{ID}](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="31f74-107">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="31f74-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31f74-108">Properties</span></span>
| <span data-ttu-id="31f74-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31f74-109">Property</span></span>     | <span data-ttu-id="31f74-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="31f74-110">Type</span></span>   |<span data-ttu-id="31f74-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="31f74-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31f74-112">ação</span><span class="sxs-lookup"><span data-stu-id="31f74-112">action</span></span>|<span data-ttu-id="31f74-113">String</span><span class="sxs-lookup"><span data-stu-id="31f74-113">String</span></span>|<span data-ttu-id="31f74-114">A ação a ser executada no elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="31f74-114">The action to perform on the target element.</span></span> <span data-ttu-id="31f74-115">Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="31f74-115">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="31f74-116">content</span><span class="sxs-lookup"><span data-stu-id="31f74-116">content</span></span>|<span data-ttu-id="31f74-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31f74-117">String</span></span>|<span data-ttu-id="31f74-118">Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo.</span><span class="sxs-lookup"><span data-stu-id="31f74-118">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="31f74-119">Se o conteúdo contiver dados binários, a solicitação deverá ser enviada `multipart/form-data` usando o tipo de conteúdo com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="31f74-119">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="31f74-120">position</span><span class="sxs-lookup"><span data-stu-id="31f74-120">position</span></span>|<span data-ttu-id="31f74-121">String</span><span class="sxs-lookup"><span data-stu-id="31f74-121">String</span></span>|<span data-ttu-id="31f74-122">O local para adicionar o conteúdo fornecido em relação ao elemento de destino.</span><span class="sxs-lookup"><span data-stu-id="31f74-122">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="31f74-123">Os valores possíveis são `after` : (padrão) `before`ou.</span><span class="sxs-lookup"><span data-stu-id="31f74-123">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="31f74-124">destino</span><span class="sxs-lookup"><span data-stu-id="31f74-124">target</span></span>|<span data-ttu-id="31f74-125">String</span><span class="sxs-lookup"><span data-stu-id="31f74-125">String</span></span>|<span data-ttu-id="31f74-126">O elemento a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="31f74-126">The element to update.</span></span> <span data-ttu-id="31f74-127">Deve ser o `#<data-id>` ou o gerado `{id}` do elemento, ou a `body` palavra- `title` chave ou.</span><span class="sxs-lookup"><span data-stu-id="31f74-127">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

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
