---
title: tipo de recurso workbookCommentReply
description: Definição do tipo de recurso workbookCommentReply
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d080f283401d9486de53095d3ad25029edbb14b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519236"
---
# <a name="workbookcommentreply-resource-type"></a><span data-ttu-id="23312-103">tipo de recurso workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="23312-103">workbookCommentReply resource type</span></span>

<span data-ttu-id="23312-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="23312-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23312-105">Representa uma resposta a um comentário do Excel.</span><span class="sxs-lookup"><span data-stu-id="23312-105">Represents a reply to an excel comment.</span></span>

## <a name="methods"></a><span data-ttu-id="23312-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="23312-106">Methods</span></span>

| <span data-ttu-id="23312-107">Método</span><span class="sxs-lookup"><span data-stu-id="23312-107">Method</span></span>       | <span data-ttu-id="23312-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23312-108">Return Type</span></span> | <span data-ttu-id="23312-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23312-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="23312-110">Listar workbookCommentReplies</span><span class="sxs-lookup"><span data-stu-id="23312-110">List workbookCommentReplies</span></span>](../api/workbookcomment-list-replies.md) | <span data-ttu-id="23312-111">coleção [workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="23312-111">[workbookCommentReply](workbookcommentreply.md) collection</span></span> | <span data-ttu-id="23312-112">Recupere uma lista de objetos workbookcommentreply.</span><span class="sxs-lookup"><span data-stu-id="23312-112">Retrieve a list of workbookcommentreply objects.</span></span> |
| [<span data-ttu-id="23312-113">Obter workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="23312-113">Get workbookCommentReply</span></span>](../api/workbookcommentreply-get.md) | [<span data-ttu-id="23312-114">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="23312-114">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="23312-115">Leia as propriedades e os relacionamentos do objeto workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="23312-115">Read properties and relationships of workbookCommentReply object.</span></span> |
| [<span data-ttu-id="23312-116">Criar workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="23312-116">Create workbookCommentReply</span></span>](../api/workbookcomment-post-replies.md) | [<span data-ttu-id="23312-117">workbookCommentReply</span><span class="sxs-lookup"><span data-stu-id="23312-117">workbookCommentReply</span></span>](workbookcommentreply.md) | <span data-ttu-id="23312-118">Criar um novo workbookCommentReply.</span><span class="sxs-lookup"><span data-stu-id="23312-118">Create a new workbookCommentReply.</span></span> |

## <a name="properties"></a><span data-ttu-id="23312-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23312-119">Properties</span></span>

| <span data-ttu-id="23312-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23312-120">Property</span></span>     | <span data-ttu-id="23312-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="23312-121">Type</span></span>        | <span data-ttu-id="23312-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="23312-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23312-123">content</span><span class="sxs-lookup"><span data-stu-id="23312-123">content</span></span>|<span data-ttu-id="23312-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23312-124">String</span></span>|<span data-ttu-id="23312-125">O conteúdo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="23312-125">The content of replied comment.</span></span>|
|<span data-ttu-id="23312-126">contentType</span><span class="sxs-lookup"><span data-stu-id="23312-126">contentType</span></span>|<span data-ttu-id="23312-127">String</span><span class="sxs-lookup"><span data-stu-id="23312-127">String</span></span>|<span data-ttu-id="23312-128">Indica o tipo do comentário respondido.</span><span class="sxs-lookup"><span data-stu-id="23312-128">Indicates the type for the replied comment.</span></span>|
|<span data-ttu-id="23312-129">id</span><span class="sxs-lookup"><span data-stu-id="23312-129">id</span></span>|<span data-ttu-id="23312-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23312-130">String</span></span>|<span data-ttu-id="23312-131">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="23312-131">Represents the comment identifier.</span></span> <span data-ttu-id="23312-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23312-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23312-133">Relações</span><span class="sxs-lookup"><span data-stu-id="23312-133">Relationships</span></span>

<span data-ttu-id="23312-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23312-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23312-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23312-135">JSON representation</span></span>

<span data-ttu-id="23312-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23312-136">The following is a JSON representation of the resource.</span></span>

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
