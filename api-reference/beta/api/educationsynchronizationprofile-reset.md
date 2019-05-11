---
title: Redefinir a sincronização em um educationSynchronizationProfile
description: Redefinir a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bd7f9112036d94b1249a413f7846f816c6c6d8ef
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938770"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="948a4-103">Redefinir a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="948a4-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="948a4-104">Redefinir a sincronização de um [perfil de sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="948a4-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="948a4-105">**Observação:** Essa operação causará a reinicialização da sincronização.</span><span class="sxs-lookup"><span data-stu-id="948a4-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="948a4-106">Os erros encontrados serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="948a4-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="948a4-107">Nenhum dado será excluído do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="948a4-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="948a4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="948a4-108">Permissions</span></span>
<span data-ttu-id="948a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="948a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="948a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="948a4-111">Permission type</span></span> | <span data-ttu-id="948a4-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="948a4-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="948a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="948a4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="948a4-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="948a4-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="948a4-115">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="948a4-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="948a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="948a4-116">Not supported.</span></span>|
|<span data-ttu-id="948a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="948a4-117">Application</span></span>|<span data-ttu-id="948a4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="948a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="948a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="948a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="948a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="948a4-120">Request headers</span></span>
| <span data-ttu-id="948a4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="948a4-121">Name</span></span>       | <span data-ttu-id="948a4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="948a4-122">Type</span></span> | <span data-ttu-id="948a4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="948a4-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="948a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="948a4-124">Authorization</span></span>  | <span data-ttu-id="948a4-125">string</span><span class="sxs-lookup"><span data-stu-id="948a4-125">string</span></span>  | <span data-ttu-id="948a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="948a4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="948a4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="948a4-128">Request body</span></span>
<span data-ttu-id="948a4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="948a4-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="948a4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="948a4-130">Response</span></span>
<span data-ttu-id="948a4-131">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="948a4-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="948a4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="948a4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="948a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="948a4-133">Request</span></span>
<span data-ttu-id="948a4-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="948a4-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="948a4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="948a4-135">Response</span></span>

<span data-ttu-id="948a4-136">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="948a4-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="948a4-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="948a4-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="948a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="948a4-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="948a4-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="948a4-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_reset-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
