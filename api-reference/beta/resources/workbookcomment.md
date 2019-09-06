---
title: tipo de recurso workbookComment
description: Representa um comentário na pasta de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a7a3427512962bd38c90faa710c501380e353f22
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775892"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="26501-103">tipo de recurso workbookComment</span><span class="sxs-lookup"><span data-stu-id="26501-103">workbookComment resource type</span></span>

<span data-ttu-id="26501-104">Representa um comentário na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="26501-104">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="26501-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="26501-105">Methods</span></span>

| <span data-ttu-id="26501-106">Método</span><span class="sxs-lookup"><span data-stu-id="26501-106">Method</span></span>       | <span data-ttu-id="26501-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26501-107">Return Type</span></span> | <span data-ttu-id="26501-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="26501-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="26501-109">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="26501-109">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="26501-110">coleção [workbookComment](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="26501-110">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="26501-111">Obtenha uma coleção de objetos **workbookComment** .</span><span class="sxs-lookup"><span data-stu-id="26501-111">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="26501-112">Obter workbookComment</span><span class="sxs-lookup"><span data-stu-id="26501-112">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="26501-113">workbookComment</span><span class="sxs-lookup"><span data-stu-id="26501-113">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="26501-114">Leia as propriedades e os relacionamentos de um objeto **workbookComment** .</span><span class="sxs-lookup"><span data-stu-id="26501-114">Read the properties and relationships of a **workbookComment** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="26501-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26501-115">Properties</span></span>

| <span data-ttu-id="26501-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26501-116">Property</span></span>     | <span data-ttu-id="26501-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="26501-117">Type</span></span>        | <span data-ttu-id="26501-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="26501-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26501-119">content</span><span class="sxs-lookup"><span data-stu-id="26501-119">content</span></span>|<span data-ttu-id="26501-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26501-120">String</span></span>|<span data-ttu-id="26501-121">O conteúdo do comentário.</span><span class="sxs-lookup"><span data-stu-id="26501-121">The content of the comment.</span></span>|
|<span data-ttu-id="26501-122">contentType</span><span class="sxs-lookup"><span data-stu-id="26501-122">contentType</span></span>|<span data-ttu-id="26501-123">String</span><span class="sxs-lookup"><span data-stu-id="26501-123">String</span></span>|<span data-ttu-id="26501-124">Indica o tipo do comentário.</span><span class="sxs-lookup"><span data-stu-id="26501-124">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="26501-125">id</span><span class="sxs-lookup"><span data-stu-id="26501-125">id</span></span>|<span data-ttu-id="26501-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26501-126">String</span></span>| <span data-ttu-id="26501-127">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="26501-127">Represents the comment identifier.</span></span> <span data-ttu-id="26501-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26501-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26501-129">Relações</span><span class="sxs-lookup"><span data-stu-id="26501-129">Relationships</span></span>

| <span data-ttu-id="26501-130">Relação</span><span class="sxs-lookup"><span data-stu-id="26501-130">Relationship</span></span> | <span data-ttu-id="26501-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26501-131">Type</span></span>        | <span data-ttu-id="26501-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26501-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26501-133">Enviar</span><span class="sxs-lookup"><span data-stu-id="26501-133">replies</span></span>|<span data-ttu-id="26501-134">coleção [workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="26501-134">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="26501-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="26501-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26501-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26501-137">JSON representation</span></span>

<span data-ttu-id="26501-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26501-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
  "baseType": "",
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
