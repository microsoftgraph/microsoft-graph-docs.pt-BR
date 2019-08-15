---
title: Continuar a sincronização em um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 538f4fd48f4a692ab0be2f9e22e49607116d2a1f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415964"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="151db-103">Continuar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="151db-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="151db-104">Retome a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="151db-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="151db-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="151db-105">Permissions</span></span>
<span data-ttu-id="151db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="151db-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="151db-108">Permission type</span></span> | <span data-ttu-id="151db-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="151db-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="151db-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="151db-110">Delegated (work or school account)</span></span> | <span data-ttu-id="151db-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="151db-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="151db-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="151db-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="151db-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="151db-113">Not supported.</span></span>|
|<span data-ttu-id="151db-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="151db-114">Application</span></span>|<span data-ttu-id="151db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="151db-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="151db-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="151db-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="151db-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="151db-117">Request headers</span></span>
| <span data-ttu-id="151db-118">Nome</span><span class="sxs-lookup"><span data-stu-id="151db-118">Name</span></span>       | <span data-ttu-id="151db-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="151db-119">Type</span></span> | <span data-ttu-id="151db-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="151db-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="151db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="151db-121">Authorization</span></span>  | <span data-ttu-id="151db-122">string</span><span class="sxs-lookup"><span data-stu-id="151db-122">string</span></span>  | <span data-ttu-id="151db-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="151db-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="151db-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="151db-125">Request body</span></span>
<span data-ttu-id="151db-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="151db-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="151db-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="151db-127">Response</span></span>
<span data-ttu-id="151db-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="151db-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="151db-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="151db-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="151db-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="151db-130">Request</span></span>
<span data-ttu-id="151db-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="151db-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="151db-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="151db-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="151db-133">C#</span><span class="sxs-lookup"><span data-stu-id="151db-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-resume-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="151db-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="151db-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-resume-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="151db-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="151db-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-resume-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="151db-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="151db-136">Response</span></span>

<span data-ttu-id="151db-137">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="151db-137">There is no response body.</span></span>

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
