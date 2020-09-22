---
title: Pausar a sincronização em um educationSynchronizationProfile
description: Pausar a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 003505dcfc00631f6d7ed9c40dbd9e4c8c3cebd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007200"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="2187e-103">Pausar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="2187e-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="2187e-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2187e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2187e-105">Pausar a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="2187e-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2187e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2187e-106">Permissions</span></span>
<span data-ttu-id="2187e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2187e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2187e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2187e-109">Permission type</span></span> | <span data-ttu-id="2187e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2187e-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2187e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2187e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2187e-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2187e-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2187e-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2187e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2187e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2187e-114">Not supported.</span></span>|
|<span data-ttu-id="2187e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2187e-115">Application</span></span>|<span data-ttu-id="2187e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2187e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2187e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2187e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="2187e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2187e-118">Request headers</span></span>
| <span data-ttu-id="2187e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2187e-119">Name</span></span>       | <span data-ttu-id="2187e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2187e-120">Type</span></span> | <span data-ttu-id="2187e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2187e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2187e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2187e-122">Authorization</span></span>  | <span data-ttu-id="2187e-123">string</span><span class="sxs-lookup"><span data-stu-id="2187e-123">string</span></span>  | <span data-ttu-id="2187e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2187e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2187e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2187e-126">Request body</span></span>
<span data-ttu-id="2187e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2187e-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2187e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2187e-128">Response</span></span>
<span data-ttu-id="2187e-129">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2187e-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2187e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2187e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2187e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2187e-131">Request</span></span>
<span data-ttu-id="2187e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2187e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2187e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2187e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="2187e-134">C#</span><span class="sxs-lookup"><span data-stu-id="2187e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2187e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2187e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2187e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2187e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2187e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2187e-137">Response</span></span>

<span data-ttu-id="2187e-138">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2187e-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```http
HTTP/1.1 200 OK
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


