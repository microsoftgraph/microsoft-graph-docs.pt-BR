---
title: Tipo de recurso patchContentCommand
description: As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.
ms.openlocfilehash: fb559a96aa5eef94dd07280b888da0df989b2363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039937"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="56d79-103">Tipo de recurso patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="56d79-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="56d79-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="56d79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56d79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56d79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56d79-106">As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="56d79-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56d79-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56d79-107">JSON representation</span></span>

<span data-ttu-id="56d79-108">Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="56d79-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="56d79-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56d79-109">Properties</span></span>
| <span data-ttu-id="56d79-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56d79-110">Property</span></span>     | <span data-ttu-id="56d79-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="56d79-111">Type</span></span>   |<span data-ttu-id="56d79-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="56d79-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56d79-113">ação</span><span class="sxs-lookup"><span data-stu-id="56d79-113">action</span></span>|<span data-ttu-id="56d79-114">String</span><span class="sxs-lookup"><span data-stu-id="56d79-114">String</span></span>|<span data-ttu-id="56d79-p102">A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.</span><span class="sxs-lookup"><span data-stu-id="56d79-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="56d79-117">content</span><span class="sxs-lookup"><span data-stu-id="56d79-117">content</span></span>|<span data-ttu-id="56d79-118">String</span><span class="sxs-lookup"><span data-stu-id="56d79-118">String</span></span>|<span data-ttu-id="56d79-p103">Uma cadeia de caracteres de HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands".</span><span class="sxs-lookup"><span data-stu-id="56d79-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="56d79-121">position</span><span class="sxs-lookup"><span data-stu-id="56d79-121">position</span></span>|<span data-ttu-id="56d79-122">String</span><span class="sxs-lookup"><span data-stu-id="56d79-122">String</span></span>|<span data-ttu-id="56d79-p104">O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before`.</span><span class="sxs-lookup"><span data-stu-id="56d79-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="56d79-125">destino</span><span class="sxs-lookup"><span data-stu-id="56d79-125">target</span></span>|<span data-ttu-id="56d79-126">String</span><span class="sxs-lookup"><span data-stu-id="56d79-126">String</span></span>|<span data-ttu-id="56d79-p105">O elemento a atualizar. Deve ser `#<data-id>` ou o `<id>` gerado do elemento ou o `body` ou a palavra-chave de `title`.</span><span class="sxs-lookup"><span data-stu-id="56d79-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->