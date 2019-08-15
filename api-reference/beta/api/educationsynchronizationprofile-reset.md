---
title: Redefinir a sincronização em um educationSynchronizationProfile
description: Redefinir a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f98548765e185d6bb3f66bbec33b50cd496c4804
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415978"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="bc858-103">Redefinir a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="bc858-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc858-104">Redefinir a sincronização de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="bc858-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="bc858-105">**Observação:** Essa operação causará a reinicialização da sincronização.</span><span class="sxs-lookup"><span data-stu-id="bc858-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="bc858-106">Os erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="bc858-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="bc858-107">Nenhum dado será excluído do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="bc858-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bc858-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc858-108">Permissions</span></span>
<span data-ttu-id="bc858-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc858-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc858-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc858-111">Permission type</span></span> | <span data-ttu-id="bc858-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc858-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bc858-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc858-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc858-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc858-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="bc858-115">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bc858-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bc858-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc858-116">Not supported.</span></span>|
|<span data-ttu-id="bc858-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc858-117">Application</span></span>|<span data-ttu-id="bc858-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc858-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc858-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc858-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="bc858-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc858-120">Request headers</span></span>
| <span data-ttu-id="bc858-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bc858-121">Name</span></span>       | <span data-ttu-id="bc858-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc858-122">Type</span></span> | <span data-ttu-id="bc858-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc858-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc858-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc858-124">Authorization</span></span>  | <span data-ttu-id="bc858-125">string</span><span class="sxs-lookup"><span data-stu-id="bc858-125">string</span></span>  | <span data-ttu-id="bc858-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc858-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc858-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc858-128">Request body</span></span>
<span data-ttu-id="bc858-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc858-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc858-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc858-130">Response</span></span>
<span data-ttu-id="bc858-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="bc858-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc858-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc858-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc858-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc858-133">Request</span></span>
<span data-ttu-id="bc858-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc858-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bc858-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc858-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc858-136">C#</span><span class="sxs-lookup"><span data-stu-id="bc858-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc858-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc858-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc858-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bc858-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bc858-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc858-139">Response</span></span>

<span data-ttu-id="bc858-140">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc858-140">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
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
