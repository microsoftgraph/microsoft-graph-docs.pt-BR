---
author: swapnil1993
title: 'contentType: unpublish'
description: Não publice um tipo de conteúdo de um site de hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ca432973337ac81f3ee8e632bb0705f26c7575ea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445859"
---
# <a name="contenttype-unpublish"></a><span data-ttu-id="24c1b-103">contentType: unpublish</span><span class="sxs-lookup"><span data-stu-id="24c1b-103">contentType: unpublish</span></span>
<span data-ttu-id="24c1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="24c1b-105">Não publice um [contentType de][] um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="24c1b-105">Unpublish a [contentType][] from a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="24c1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24c1b-106">Permissions</span></span>

<span data-ttu-id="24c1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="24c1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24c1b-109">Permission type</span></span>      | <span data-ttu-id="24c1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24c1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24c1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24c1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24c1b-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="24c1b-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="24c1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24c1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24c1b-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="24c1b-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="24c1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24c1b-115">Application</span></span> | <span data-ttu-id="24c1b-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="24c1b-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24c1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24c1b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

><span data-ttu-id="24c1b-118">**Observação:** O siteId representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="24c1b-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24c1b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24c1b-119">Request headers</span></span>
|<span data-ttu-id="24c1b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="24c1b-120">Name</span></span>|<span data-ttu-id="24c1b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="24c1b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24c1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="24c1b-122">Authorization</span></span>|<span data-ttu-id="24c1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24c1b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c1b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24c1b-125">Request body</span></span>
<span data-ttu-id="24c1b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24c1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c1b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c1b-127">Response</span></span>

<span data-ttu-id="24c1b-128">Se tiver êxito, este método retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="24c1b-128">If successful, this method returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="24c1b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24c1b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c1b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24c1b-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

### <a name="response"></a><span data-ttu-id="24c1b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c1b-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
