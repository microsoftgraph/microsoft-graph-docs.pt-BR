---
title: Tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dc25b02005e0f419fbb878005006f155f1f99e72
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159427"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="d269c-103">Tipo de recurso workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d269c-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="d269c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d269c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d269c-105">Representa uma resposta a um comentário do Excel.</span><span class="sxs-lookup"><span data-stu-id="d269c-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="d269c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d269c-106">Methods</span></span>

| <span data-ttu-id="d269c-107">Método</span><span class="sxs-lookup"><span data-stu-id="d269c-107">Method</span></span>       | <span data-ttu-id="d269c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d269c-108">Return Type</span></span> | <span data-ttu-id="d269c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d269c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d269c-110">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="d269c-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="d269c-111">[coleção workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="d269c-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="d269c-112">Recupere uma lista de objetos workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="d269c-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="d269c-113">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d269c-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="d269c-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d269c-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d269c-115">Leia as propriedades e as relações do objeto workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="d269c-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="d269c-116">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d269c-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="d269c-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="d269c-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="d269c-118">Crie uma nova workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="d269c-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="d269c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d269c-119">Properties</span></span>

| <span data-ttu-id="d269c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d269c-120">Property</span></span>     | <span data-ttu-id="d269c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d269c-121">Type</span></span>        | <span data-ttu-id="d269c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d269c-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d269c-123">content</span><span class="sxs-lookup"><span data-stu-id="d269c-123">content</span></span>|<span data-ttu-id="d269c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d269c-124">String</span></span>|<span data-ttu-id="d269c-125">O conteúdo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="d269c-125">The content of replied comment.</span></span>|
|<span data-ttu-id="d269c-126">contentType</span><span class="sxs-lookup"><span data-stu-id="d269c-126">contentType</span></span>|<span data-ttu-id="d269c-127">String</span><span class="sxs-lookup"><span data-stu-id="d269c-127">String</span></span>|<span data-ttu-id="d269c-128">Indica o tipo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="d269c-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="d269c-129">id</span><span class="sxs-lookup"><span data-stu-id="d269c-129">id</span></span>|<span data-ttu-id="d269c-130">String</span><span class="sxs-lookup"><span data-stu-id="d269c-130">String</span></span>|<span data-ttu-id="d269c-131">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="d269c-131">Represents the comment identifier.</span></span> <span data-ttu-id="d269c-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d269c-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d269c-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d269c-133">Relationships</span></span>

<span data-ttu-id="d269c-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d269c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d269c-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d269c-135">JSON representation</span></span>

<span data-ttu-id="d269c-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d269c-136">The following is a JSON representation of the resource.</span></span>

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


