---
title: tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0a4dfc215eec435c67f1259a85e899db4dfb2b63
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775899"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="9a883-103">tipo de recurso workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9a883-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="9a883-104">Representa uma resposta a um comentário do Excel.</span><span class="sxs-lookup"><span data-stu-id="9a883-104">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="9a883-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a883-105">Methods</span></span>

| <span data-ttu-id="9a883-106">Método</span><span class="sxs-lookup"><span data-stu-id="9a883-106">Method</span></span>       | <span data-ttu-id="9a883-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a883-107">Return Type</span></span> | <span data-ttu-id="9a883-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a883-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9a883-109">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="9a883-109">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="9a883-110">coleção [workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="9a883-110">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="9a883-111">Recupere uma lista de objetos workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="9a883-111">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="9a883-112">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9a883-112">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="9a883-113">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9a883-113">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="9a883-114">Leia as propriedades e os relacionamentos do objeto workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="9a883-114">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="9a883-115">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9a883-115">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="9a883-116">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="9a883-116">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="9a883-117">Criar um novo workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="9a883-117">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a883-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a883-118">Properties</span></span>

| <span data-ttu-id="9a883-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a883-119">Property</span></span>     | <span data-ttu-id="9a883-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a883-120">Type</span></span>        | <span data-ttu-id="9a883-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a883-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a883-122">content</span><span class="sxs-lookup"><span data-stu-id="9a883-122">content</span></span>|<span data-ttu-id="9a883-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a883-123">String</span></span>|<span data-ttu-id="9a883-124">O conteúdo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="9a883-124">The content of replied comment.</span></span>|
|<span data-ttu-id="9a883-125">contentType</span><span class="sxs-lookup"><span data-stu-id="9a883-125">contentType</span></span>|<span data-ttu-id="9a883-126">String</span><span class="sxs-lookup"><span data-stu-id="9a883-126">String</span></span>|<span data-ttu-id="9a883-127">Indica o tipo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="9a883-127">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="9a883-128">id</span><span class="sxs-lookup"><span data-stu-id="9a883-128">id</span></span>|<span data-ttu-id="9a883-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a883-129">String</span></span>|<span data-ttu-id="9a883-130">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="9a883-130">Represents the comment identifier.</span></span> <span data-ttu-id="9a883-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a883-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a883-132">Relações</span><span class="sxs-lookup"><span data-stu-id="9a883-132">Relationships</span></span>

<span data-ttu-id="9a883-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a883-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a883-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a883-134">JSON representation</span></span>

<span data-ttu-id="9a883-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a883-135">The following is a JSON representation of the resource.</span></span>

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
