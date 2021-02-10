---
title: Tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7c47a6eb7abf8bf675dd8be35db6a96e511dbbcf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158034"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="3e147-103">Tipo de recurso workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="3e147-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="3e147-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e147-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e147-105">Representa uma resposta a um comentário do Excel.</span><span class="sxs-lookup"><span data-stu-id="3e147-105">Represents a reply to an Excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="3e147-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3e147-106">Methods</span></span>

| <span data-ttu-id="3e147-107">Método</span><span class="sxs-lookup"><span data-stu-id="3e147-107">Method</span></span>       | <span data-ttu-id="3e147-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e147-108">Return Type</span></span> | <span data-ttu-id="3e147-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e147-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3e147-110">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="3e147-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="3e147-111">[coleção workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="3e147-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="3e147-112">Recupere uma lista de objetos workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="3e147-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="3e147-113">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="3e147-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="3e147-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="3e147-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="3e147-115">Leia as propriedades e as relações do objeto workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="3e147-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="3e147-116">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="3e147-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="3e147-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="3e147-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="3e147-118">Crie uma nova workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="3e147-118">Create a new workbookCommentReply.</span></span> |
## <a name="properties"></a><span data-ttu-id="3e147-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e147-119">Properties</span></span>

| <span data-ttu-id="3e147-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e147-120">Property</span></span>     | <span data-ttu-id="3e147-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e147-121">Type</span></span>        | <span data-ttu-id="3e147-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e147-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e147-123">content</span><span class="sxs-lookup"><span data-stu-id="3e147-123">content</span></span>|<span data-ttu-id="3e147-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e147-124">String</span></span>|<span data-ttu-id="3e147-125">O conteúdo de uma resposta de comentário.</span><span class="sxs-lookup"><span data-stu-id="3e147-125">The content of a comment reply.</span></span>|
|<span data-ttu-id="3e147-126">contentType</span><span class="sxs-lookup"><span data-stu-id="3e147-126">contentType</span></span>|<span data-ttu-id="3e147-127">String</span><span class="sxs-lookup"><span data-stu-id="3e147-127">String</span></span>|<span data-ttu-id="3e147-128">Indica o tipo da resposta do comentário.</span><span class="sxs-lookup"><span data-stu-id="3e147-128">Indicates the type for the comment reply.</span></span>|
|<span data-ttu-id="3e147-129">id</span><span class="sxs-lookup"><span data-stu-id="3e147-129">id</span></span>|<span data-ttu-id="3e147-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e147-130">String</span></span>|<span data-ttu-id="3e147-131">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="3e147-131">Represents the comment identifier.</span></span> <span data-ttu-id="3e147-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3e147-132">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3e147-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3e147-133">Relationships</span></span>

<span data-ttu-id="3e147-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e147-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e147-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e147-135">JSON representation</span></span>

<span data-ttu-id="3e147-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e147-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
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

