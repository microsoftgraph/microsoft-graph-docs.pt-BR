---
title: tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8c93dcb4a4ccd1289de8d19b8970cbf0b87e80cc
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775731"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="979c6-103">tipo de recurso workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="979c6-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="979c6-104">Representa uma resposta a um comentário do Excel.</span><span class="sxs-lookup"><span data-stu-id="979c6-104">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="979c6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="979c6-105">Methods</span></span>

| <span data-ttu-id="979c6-106">Método</span><span class="sxs-lookup"><span data-stu-id="979c6-106">Method</span></span>       | <span data-ttu-id="979c6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="979c6-107">Return Type</span></span> | <span data-ttu-id="979c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="979c6-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="979c6-109">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="979c6-109">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="979c6-110">coleção [workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="979c6-110">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="979c6-111">Recupere uma lista de objetos workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="979c6-111">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="979c6-112">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="979c6-112">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="979c6-113">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="979c6-113">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="979c6-114">Leia as propriedades e os relacionamentos do objeto workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="979c6-114">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="979c6-115">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="979c6-115">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="979c6-116">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="979c6-116">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="979c6-117">Criar um novo workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="979c6-117">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="979c6-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="979c6-118">Properties</span></span>

| <span data-ttu-id="979c6-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="979c6-119">Property</span></span>     | <span data-ttu-id="979c6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="979c6-120">Type</span></span>        | <span data-ttu-id="979c6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="979c6-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="979c6-122">content</span><span class="sxs-lookup"><span data-stu-id="979c6-122">content</span></span>|<span data-ttu-id="979c6-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="979c6-123">String</span></span>|<span data-ttu-id="979c6-124">O conteúdo de uma resposta de comentário.</span><span class="sxs-lookup"><span data-stu-id="979c6-124">The content of a comment reply.</span></span>|
|<span data-ttu-id="979c6-125">contentType</span><span class="sxs-lookup"><span data-stu-id="979c6-125">contentType</span></span>|<span data-ttu-id="979c6-126">String</span><span class="sxs-lookup"><span data-stu-id="979c6-126">String</span></span>|<span data-ttu-id="979c6-127">Indica o tipo da resposta de comentário.</span><span class="sxs-lookup"><span data-stu-id="979c6-127">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="979c6-128">id</span><span class="sxs-lookup"><span data-stu-id="979c6-128">id</span></span>|<span data-ttu-id="979c6-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="979c6-129">String</span></span>|<span data-ttu-id="979c6-130">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="979c6-130">Represents the comment identifier.</span></span> <span data-ttu-id="979c6-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="979c6-131">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="979c6-132">Relações</span><span class="sxs-lookup"><span data-stu-id="979c6-132">Relationships</span></span>

<span data-ttu-id="979c6-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="979c6-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="979c6-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="979c6-134">JSON representation</span></span>

<span data-ttu-id="979c6-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="979c6-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
