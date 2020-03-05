---
title: Continuar a sincronização em um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5285edf11ae84100c4a5f99ccf9841007999cf8f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424376"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="c237d-103">Continuar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c237d-103">Resume sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="c237d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c237d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c237d-105">Retome a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="c237d-105">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c237d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c237d-106">Permissions</span></span>
<span data-ttu-id="c237d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c237d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c237d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c237d-109">Permission type</span></span> | <span data-ttu-id="c237d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c237d-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c237d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c237d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c237d-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c237d-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c237d-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c237d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c237d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c237d-114">Not supported.</span></span>|
|<span data-ttu-id="c237d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c237d-115">Application</span></span>|<span data-ttu-id="c237d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c237d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c237d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c237d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="c237d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c237d-118">Request headers</span></span>
| <span data-ttu-id="c237d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c237d-119">Name</span></span>       | <span data-ttu-id="c237d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c237d-120">Type</span></span> | <span data-ttu-id="c237d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c237d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c237d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c237d-122">Authorization</span></span>  | <span data-ttu-id="c237d-123">string</span><span class="sxs-lookup"><span data-stu-id="c237d-123">string</span></span>  | <span data-ttu-id="c237d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c237d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c237d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c237d-126">Request body</span></span>
<span data-ttu-id="c237d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c237d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c237d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c237d-128">Response</span></span>
<span data-ttu-id="c237d-129">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c237d-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c237d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c237d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c237d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c237d-131">Request</span></span>
<span data-ttu-id="c237d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c237d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c237d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c237d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="c"></a>[<span data-ttu-id="c237d-134">C#</span><span class="sxs-lookup"><span data-stu-id="c237d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c237d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c237d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c237d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c237d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c237d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c237d-137">Response</span></span>

<span data-ttu-id="c237d-138">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c237d-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
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
