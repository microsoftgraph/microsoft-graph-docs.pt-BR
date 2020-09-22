---
title: Redefinir a sincronização em um educationSynchronizationProfile
description: Redefinir a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00ed8f14dd2b84b0fab48c31dd352d53fffc805a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007093"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="36731-103">Redefinir a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="36731-103">Reset sync on an educationSynchronizationProfile</span></span>

<span data-ttu-id="36731-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36731-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36731-105">Redefinir a sincronização de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="36731-105">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="36731-106">**Observação:** Essa operação causará a reinicialização da sincronização.</span><span class="sxs-lookup"><span data-stu-id="36731-106">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="36731-107">Os erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="36731-107">Any errors encountered will be deleted.</span></span> <span data-ttu-id="36731-108">Nenhum dado será excluído do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="36731-108">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="36731-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="36731-109">Permissions</span></span>
<span data-ttu-id="36731-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36731-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36731-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36731-112">Permission type</span></span> | <span data-ttu-id="36731-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="36731-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="36731-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36731-114">Delegated (work or school account)</span></span> | <span data-ttu-id="36731-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36731-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="36731-116">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="36731-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="36731-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36731-117">Not supported.</span></span>|
|<span data-ttu-id="36731-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36731-118">Application</span></span>|<span data-ttu-id="36731-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36731-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36731-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36731-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="36731-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36731-121">Request headers</span></span>
| <span data-ttu-id="36731-122">Nome</span><span class="sxs-lookup"><span data-stu-id="36731-122">Name</span></span>       | <span data-ttu-id="36731-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="36731-123">Type</span></span> | <span data-ttu-id="36731-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="36731-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36731-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="36731-125">Authorization</span></span>  | <span data-ttu-id="36731-126">string</span><span class="sxs-lookup"><span data-stu-id="36731-126">string</span></span>  | <span data-ttu-id="36731-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36731-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36731-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36731-129">Request body</span></span>
<span data-ttu-id="36731-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36731-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="36731-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="36731-131">Response</span></span>
<span data-ttu-id="36731-132">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="36731-132">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36731-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36731-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36731-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36731-134">Request</span></span>
<span data-ttu-id="36731-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36731-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36731-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="36731-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```
# <a name="c"></a>[<span data-ttu-id="36731-137">C#</span><span class="sxs-lookup"><span data-stu-id="36731-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-reset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36731-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36731-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-reset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36731-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36731-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-reset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36731-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="36731-140">Response</span></span>

<span data-ttu-id="36731-141">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36731-141">There is no response body.</span></span>

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


