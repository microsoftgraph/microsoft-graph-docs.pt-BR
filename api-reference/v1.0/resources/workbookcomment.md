---
title: tipo de recurso workbookComment
description: Definição do tipo de recurso workbookComment
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b89f7b1ed2ca1ca833d8d5bae72d74a58b714997
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015166"
---
# <a name="workbookcomment-resource-type"></a><span data-ttu-id="8b386-103">tipo de recurso workbookComment</span><span class="sxs-lookup"><span data-stu-id="8b386-103">workbookComment resource type</span></span>

<span data-ttu-id="8b386-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b386-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b386-105">Representa um comentário na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8b386-105">Represents a comment in workbook.</span></span>

## <a name="methods"></a><span data-ttu-id="8b386-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8b386-106">Methods</span></span>

| <span data-ttu-id="8b386-107">Método</span><span class="sxs-lookup"><span data-stu-id="8b386-107">Method</span></span>       | <span data-ttu-id="8b386-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b386-108">Return Type</span></span> | <span data-ttu-id="8b386-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b386-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8b386-110">Listar workbookComments</span><span class="sxs-lookup"><span data-stu-id="8b386-110">List workbookComments</span></span>](../api/workbook-list-comments.md) | <span data-ttu-id="8b386-111">coleção [workbookComment](workbookComment.md)</span><span class="sxs-lookup"><span data-stu-id="8b386-111">[workbookComment](workbookComment.md) collection</span></span> | <span data-ttu-id="8b386-112">Obtenha uma coleção de objetos **workbookComment** .</span><span class="sxs-lookup"><span data-stu-id="8b386-112">Get a **workbookComment** object collection.</span></span> |
| [<span data-ttu-id="8b386-113">Obter workbookComment</span><span class="sxs-lookup"><span data-stu-id="8b386-113">Get workbookComment</span></span>](../api/workbookcomment-get.md) | [<span data-ttu-id="8b386-114">workbookComment</span><span class="sxs-lookup"><span data-stu-id="8b386-114">workbookComment</span></span>](workbookcomment.md) | <span data-ttu-id="8b386-115">Leia as propriedades e os relacionamentos de um objeto **workbookComment** .</span><span class="sxs-lookup"><span data-stu-id="8b386-115">Read the properties and relationships of a **workbookComment** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8b386-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b386-116">Properties</span></span>

| <span data-ttu-id="8b386-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b386-117">Property</span></span>     | <span data-ttu-id="8b386-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b386-118">Type</span></span>        | <span data-ttu-id="8b386-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b386-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b386-120">content</span><span class="sxs-lookup"><span data-stu-id="8b386-120">content</span></span>|<span data-ttu-id="8b386-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b386-121">String</span></span>|<span data-ttu-id="8b386-122">O conteúdo de comment.</span><span class="sxs-lookup"><span data-stu-id="8b386-122">The content of comment.</span></span>|
|<span data-ttu-id="8b386-123">contentType</span><span class="sxs-lookup"><span data-stu-id="8b386-123">contentType</span></span>|<span data-ttu-id="8b386-124">String</span><span class="sxs-lookup"><span data-stu-id="8b386-124">String</span></span>|<span data-ttu-id="8b386-125">Indica o tipo do comentário.</span><span class="sxs-lookup"><span data-stu-id="8b386-125">Indicates the type for the comment.</span></span>|
|<span data-ttu-id="8b386-126">id</span><span class="sxs-lookup"><span data-stu-id="8b386-126">id</span></span>|<span data-ttu-id="8b386-127">String</span><span class="sxs-lookup"><span data-stu-id="8b386-127">String</span></span>| <span data-ttu-id="8b386-128">Representa o identificador de comentário.</span><span class="sxs-lookup"><span data-stu-id="8b386-128">Represents the comment identifier.</span></span> <span data-ttu-id="8b386-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8b386-129">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b386-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8b386-130">Relationships</span></span>

| <span data-ttu-id="8b386-131">Relação</span><span class="sxs-lookup"><span data-stu-id="8b386-131">Relationship</span></span> | <span data-ttu-id="8b386-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b386-132">Type</span></span>        | <span data-ttu-id="8b386-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b386-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b386-134">Enviar</span><span class="sxs-lookup"><span data-stu-id="8b386-134">replies</span></span>|<span data-ttu-id="8b386-135">coleção [workbookCommentReply](workbookcommentreply.md)</span><span class="sxs-lookup"><span data-stu-id="8b386-135">[workbookCommentReply](workbookcommentreply.md) collection</span></span>| <span data-ttu-id="8b386-p102">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8b386-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b386-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b386-138">JSON representation</span></span>

<span data-ttu-id="8b386-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b386-139">The following is a JSON representation of the resource.</span></span>

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

