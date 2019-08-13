---
title: Pausar a sincronização em um educationSynchronizationProfile
description: Pausar a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ccfbb67ed6363f39120b2b6295dfd1624d38e133
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325348"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="59362-103">Pausar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="59362-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59362-104">Pausar a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="59362-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="59362-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="59362-105">Permissions</span></span>
<span data-ttu-id="59362-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59362-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59362-108">Permission type</span></span> | <span data-ttu-id="59362-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="59362-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="59362-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59362-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59362-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59362-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="59362-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="59362-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="59362-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59362-113">Not supported.</span></span>|
|<span data-ttu-id="59362-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59362-114">Application</span></span>|<span data-ttu-id="59362-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59362-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59362-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59362-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="59362-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59362-117">Request headers</span></span>
| <span data-ttu-id="59362-118">Nome</span><span class="sxs-lookup"><span data-stu-id="59362-118">Name</span></span>       | <span data-ttu-id="59362-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="59362-119">Type</span></span> | <span data-ttu-id="59362-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="59362-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59362-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59362-121">Authorization</span></span>  | <span data-ttu-id="59362-122">string</span><span class="sxs-lookup"><span data-stu-id="59362-122">string</span></span>  | <span data-ttu-id="59362-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59362-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59362-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59362-125">Request body</span></span>
<span data-ttu-id="59362-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59362-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="59362-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="59362-127">Response</span></span>
<span data-ttu-id="59362-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="59362-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="59362-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59362-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59362-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59362-130">Request</span></span>
<span data-ttu-id="59362-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59362-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59362-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="59362-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59362-133">C#</span><span class="sxs-lookup"><span data-stu-id="59362-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-synchronizationprofile-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59362-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59362-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-synchronizationprofile-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59362-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="59362-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-synchronizationprofile-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59362-136">Java</span><span class="sxs-lookup"><span data-stu-id="59362-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-synchronizationprofile-pause-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59362-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="59362-137">Response</span></span>

<span data-ttu-id="59362-138">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59362-138">There is no response body.</span></span>

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
