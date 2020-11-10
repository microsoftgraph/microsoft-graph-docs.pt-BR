---
title: Redefinir a sincronização em um educationSynchronizationProfile
description: Redefinir a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 517dc5e2fddf0c959215fb69621e0bb99bad75e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965827"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="53117-103">Redefinir a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="53117-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="53117-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53117-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53117-105">Redefinir a sincronização de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="53117-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="53117-106">**Observação:** Essa operação causará a reinicialização da sincronização.</span><span class="sxs-lookup"><span data-stu-id="53117-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="53117-107">Os erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="53117-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="53117-108">Nenhum dado será excluído do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="53117-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="53117-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="53117-109">Permissions</span></span>
<span data-ttu-id="53117-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53117-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53117-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53117-112">Permission type</span></span> | <span data-ttu-id="53117-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="53117-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="53117-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53117-114">Delegated (work or school account)</span></span> | <span data-ttu-id="53117-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53117-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="53117-116">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="53117-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="53117-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53117-117">Not supported.</span></span>|
|<span data-ttu-id="53117-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53117-118">Application</span></span>|<span data-ttu-id="53117-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53117-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53117-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53117-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="53117-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53117-121">Request headers</span></span>
| <span data-ttu-id="53117-122">Nome</span><span class="sxs-lookup"><span data-stu-id="53117-122">Name</span></span>       | <span data-ttu-id="53117-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="53117-123">Type</span></span> | <span data-ttu-id="53117-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="53117-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53117-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="53117-125">Authorization</span></span>  | <span data-ttu-id="53117-126">string</span><span class="sxs-lookup"><span data-stu-id="53117-126">string</span></span>  | <span data-ttu-id="53117-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53117-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53117-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53117-129">Request body</span></span>
<span data-ttu-id="53117-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53117-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53117-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="53117-131">Response</span></span>
<span data-ttu-id="53117-132">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="53117-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="53117-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53117-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53117-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53117-134">Request</span></span>
<span data-ttu-id="53117-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="53117-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53117-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="53117-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="53117-137">C#</span><span class="sxs-lookup"><span data-stu-id="53117-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53117-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53117-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53117-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53117-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53117-140">Java</span><span class="sxs-lookup"><span data-stu-id="53117-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-reset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53117-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="53117-141">Response</span></span>

<span data-ttu-id="53117-142">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="53117-142">There is no response body.</span></span>

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


