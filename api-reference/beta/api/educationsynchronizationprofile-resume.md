---
title: Continuar a sincronização em um educationSynchronizationProfile
description: Retome a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b4abb054763416e65f99da14aaa1e2ea1db1eb15
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587446"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="d7b46-103">Continuar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="d7b46-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b46-104">Retome a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="d7b46-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7b46-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7b46-105">Permissions</span></span>
<span data-ttu-id="d7b46-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7b46-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7b46-108">Permission type</span></span> | <span data-ttu-id="d7b46-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7b46-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="d7b46-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7b46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7b46-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7b46-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="d7b46-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d7b46-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d7b46-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7b46-113">Not supported.</span></span>|
|<span data-ttu-id="d7b46-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7b46-114">Application</span></span>|<span data-ttu-id="d7b46-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7b46-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7b46-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7b46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="d7b46-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b46-117">Request headers</span></span>
| <span data-ttu-id="d7b46-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d7b46-118">Name</span></span>       | <span data-ttu-id="d7b46-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7b46-119">Type</span></span> | <span data-ttu-id="d7b46-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7b46-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7b46-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7b46-121">Authorization</span></span>  | <span data-ttu-id="d7b46-122">string</span><span class="sxs-lookup"><span data-stu-id="d7b46-122">string</span></span>  | <span data-ttu-id="d7b46-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7b46-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d7b46-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b46-125">Request body</span></span>
<span data-ttu-id="d7b46-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7b46-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d7b46-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7b46-127">Response</span></span>
<span data-ttu-id="d7b46-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d7b46-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7b46-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7b46-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7b46-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7b46-130">Request</span></span>
<span data-ttu-id="d7b46-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7b46-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="d7b46-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7b46-132">Response</span></span>

<span data-ttu-id="d7b46-133">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7b46-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7b46-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d7b46-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7b46-135">Basic</span><span class="sxs-lookup"><span data-stu-id="d7b46-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7b46-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7b46-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_resume-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
