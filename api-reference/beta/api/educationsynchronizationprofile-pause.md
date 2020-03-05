---
title: Pausar a sincronização em um educationSynchronizationProfile
description: Pausar a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71012e82fdb3e695d1ccf4e61dc9433c7fa2ebc1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424453"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="eaa25-103">Pausar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="eaa25-103">Pause sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="eaa25-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eaa25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaa25-105">Pausar a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="eaa25-105">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa25-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaa25-106">Permissions</span></span>
<span data-ttu-id="eaa25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eaa25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaa25-109">Permission type</span></span> | <span data-ttu-id="eaa25-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaa25-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="eaa25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaa25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa25-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eaa25-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="eaa25-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="eaa25-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eaa25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaa25-114">Not supported.</span></span>|
|<span data-ttu-id="eaa25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaa25-115">Application</span></span>|<span data-ttu-id="eaa25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaa25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaa25-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="eaa25-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaa25-118">Request headers</span></span>
| <span data-ttu-id="eaa25-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eaa25-119">Name</span></span>       | <span data-ttu-id="eaa25-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaa25-120">Type</span></span> | <span data-ttu-id="eaa25-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaa25-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eaa25-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaa25-122">Authorization</span></span>  | <span data-ttu-id="eaa25-123">string</span><span class="sxs-lookup"><span data-stu-id="eaa25-123">string</span></span>  | <span data-ttu-id="eaa25-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaa25-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eaa25-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaa25-126">Request body</span></span>
<span data-ttu-id="eaa25-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eaa25-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eaa25-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaa25-128">Response</span></span>
<span data-ttu-id="eaa25-129">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="eaa25-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eaa25-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaa25-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa25-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaa25-131">Request</span></span>
<span data-ttu-id="eaa25-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaa25-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eaa25-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaa25-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="c"></a>[<span data-ttu-id="eaa25-134">C#</span><span class="sxs-lookup"><span data-stu-id="eaa25-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eaa25-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaa25-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eaa25-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eaa25-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="eaa25-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaa25-137">Response</span></span>

<span data-ttu-id="eaa25-138">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eaa25-138">There is no response body.</span></span>

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
