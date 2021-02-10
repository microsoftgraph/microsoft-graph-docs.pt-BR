---
title: Tipo de recurso workbookComment
description: Definição do tipo de recurso workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 24cce9a392f9d5b9cfcdfc35e0c87ade16d760d7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158048"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="a2ac4-103">Tipo de recurso workbookComment</span><span class="sxs-lookup"><span data-stu-id="a2ac4-103">workbookComment resource type</span></span>

<span data-ttu-id="a2ac4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ac4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2ac4-105">Representa um comentário na área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="a2ac4-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2ac4-106">Methods</span></span>

| <span data-ttu-id="a2ac4-107">Método</span><span class="sxs-lookup"><span data-stu-id="a2ac4-107">Method</span></span>       | <span data-ttu-id="a2ac4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2ac4-108">Return Type</span></span> | <span data-ttu-id="a2ac4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ac4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a2ac4-110">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="a2ac4-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="a2ac4-111">[coleção workbookComment](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="a2ac4-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="a2ac4-112">Obter uma **coleção de objetos workbookComment.**</span><span class="sxs-lookup"><span data-stu-id="a2ac4-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="a2ac4-113">Obter workbookComment</span><span class="sxs-lookup"><span data-stu-id="a2ac4-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="a2ac4-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="a2ac4-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="a2ac4-115">Leia as propriedades e os relacionamentos de um **objeto workbookComment.**</span><span class="sxs-lookup"><span data-stu-id="a2ac4-115">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2ac4-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2ac4-116">Properties</span></span>

| <span data-ttu-id="a2ac4-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2ac4-117">Property</span></span>     | <span data-ttu-id="a2ac4-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2ac4-118">Type</span></span>        | <span data-ttu-id="a2ac4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ac4-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2ac4-120">content</span><span class="sxs-lookup"><span data-stu-id="a2ac4-120">content</span></span>|<span data-ttu-id="a2ac4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2ac4-121">String</span></span>|<span data-ttu-id="a2ac4-122">O conteúdo do comentário.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-122">The content of comment.</span></span>|
|<span data-ttu-id="a2ac4-123">contentType</span><span class="sxs-lookup"><span data-stu-id="a2ac4-123">contentType</span></span>|<span data-ttu-id="a2ac4-124">String</span><span class="sxs-lookup"><span data-stu-id="a2ac4-124">String</span></span>|<span data-ttu-id="a2ac4-125">Indica o tipo do comentário.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="a2ac4-126">id</span><span class="sxs-lookup"><span data-stu-id="a2ac4-126">id</span></span>|<span data-ttu-id="a2ac4-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2ac4-127">String</span></span>| <span data-ttu-id="a2ac4-128">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-128">Represents the comment identifier.</span></span> <span data-ttu-id="a2ac4-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2ac4-130">Relações</span><span class="sxs-lookup"><span data-stu-id="a2ac4-130">Relationships</span></span>

| <span data-ttu-id="a2ac4-131">Relação</span><span class="sxs-lookup"><span data-stu-id="a2ac4-131">Relationship</span></span> | <span data-ttu-id="a2ac4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2ac4-132">Type</span></span>        | <span data-ttu-id="a2ac4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ac4-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2ac4-134">respostas</span><span class="sxs-lookup"><span data-stu-id="a2ac4-134">replies</span></span>|<span data-ttu-id="a2ac4-135">[coleção workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="a2ac4-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="a2ac4-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2ac4-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2ac4-138">JSON representation</span></span>

<span data-ttu-id="a2ac4-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2ac4-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

