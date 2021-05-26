---
title: Retomar a sincronização em um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escolares específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0f1cd4ca3e1569825bda00a16723801521d1bc08
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664724"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="1326b-103">Retomar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="1326b-103">Resume sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="1326b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1326b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1326b-105">Retome a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolares específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="1326b-105">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1326b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1326b-106">Permissions</span></span>
<span data-ttu-id="1326b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1326b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1326b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1326b-109">Permission type</span></span> | <span data-ttu-id="1326b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1326b-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1326b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1326b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1326b-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1326b-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1326b-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1326b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1326b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1326b-114">Not supported.</span></span>|
|<span data-ttu-id="1326b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1326b-115">Application</span></span>|<span data-ttu-id="1326b-116">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1326b-116">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1326b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1326b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="1326b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1326b-118">Request headers</span></span>
| <span data-ttu-id="1326b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1326b-119">Name</span></span>       | <span data-ttu-id="1326b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1326b-120">Type</span></span> | <span data-ttu-id="1326b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1326b-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1326b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1326b-122">Authorization</span></span>  | <span data-ttu-id="1326b-123">string</span><span class="sxs-lookup"><span data-stu-id="1326b-123">string</span></span>  | <span data-ttu-id="1326b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1326b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1326b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1326b-126">Request body</span></span>
<span data-ttu-id="1326b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1326b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1326b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1326b-128">Response</span></span>
<span data-ttu-id="1326b-129">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1326b-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1326b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1326b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1326b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1326b-131">Request</span></span>
<span data-ttu-id="1326b-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1326b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1326b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1326b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="c"></a>[<span data-ttu-id="1326b-134">C#</span><span class="sxs-lookup"><span data-stu-id="1326b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1326b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1326b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1326b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1326b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1326b-137">Java</span><span class="sxs-lookup"><span data-stu-id="1326b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-resume-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1326b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1326b-138">Response</span></span>

<span data-ttu-id="1326b-139">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1326b-139">There is no response body.</span></span>

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


