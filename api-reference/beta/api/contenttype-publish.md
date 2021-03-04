---
author: swapnil1993
title: 'contentType: publish'
description: Publique um tipo de conteúdo presente no site do hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 072fb067114f9693f18a63c2d1e881fa55a7ca6b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445860"
---
# <a name="contenttype-publish"></a><span data-ttu-id="385d0-103">contentType: publish</span><span class="sxs-lookup"><span data-stu-id="385d0-103">contentType: publish</span></span>
<span data-ttu-id="385d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="385d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="385d0-105">Publica um [contentType][] presente no site do hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="385d0-105">Publishes a [contentType][] present in content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="385d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="385d0-106">Permissions</span></span>

<span data-ttu-id="385d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="385d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="385d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="385d0-109">Permission type</span></span>      | <span data-ttu-id="385d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="385d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="385d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="385d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="385d0-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="385d0-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="385d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="385d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="385d0-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="385d0-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="385d0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="385d0-115">Application</span></span> | <span data-ttu-id="385d0-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="385d0-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="385d0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="385d0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="385d0-118">**Observação:** O siteId representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="385d0-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="385d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="385d0-119">Request headers</span></span>
|<span data-ttu-id="385d0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="385d0-120">Name</span></span>|<span data-ttu-id="385d0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="385d0-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="385d0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="385d0-122">Authorization</span></span>|<span data-ttu-id="385d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="385d0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="385d0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="385d0-125">Request body</span></span>
<span data-ttu-id="385d0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="385d0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="385d0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="385d0-127">Response</span></span>
<span data-ttu-id="385d0-128">Se tiver êxito, essa chamada retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="385d0-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="385d0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="385d0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="385d0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="385d0-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```

### <a name="response"></a><span data-ttu-id="385d0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="385d0-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
