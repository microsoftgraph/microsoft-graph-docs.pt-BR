---
title: Pausar a sincronização em um educationSynchronizationProfile
description: Pausar a sincronização de um perfil de sincronização de dados escolar específico no locatário.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 93628e40bd75ad1c19581ff4f30a771e4350d206
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259525"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="4052a-103">Pausar a sincronização em um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4052a-103">Pause sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4052a-104">Pausar a sincronização de um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados escolar específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="4052a-104">Pause the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4052a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4052a-105">Permissions</span></span>
<span data-ttu-id="4052a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4052a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4052a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4052a-108">Permission type</span></span> | <span data-ttu-id="4052a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4052a-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4052a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4052a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4052a-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4052a-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4052a-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4052a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4052a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4052a-113">Not supported.</span></span>|
|<span data-ttu-id="4052a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4052a-114">Application</span></span>|<span data-ttu-id="4052a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4052a-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4052a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4052a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a><span data-ttu-id="4052a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-117">Request headers</span></span>
| <span data-ttu-id="4052a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4052a-118">Name</span></span>       | <span data-ttu-id="4052a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4052a-119">Type</span></span> | <span data-ttu-id="4052a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4052a-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4052a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4052a-121">Authorization</span></span>  | <span data-ttu-id="4052a-122">string</span><span class="sxs-lookup"><span data-stu-id="4052a-122">string</span></span>  | <span data-ttu-id="4052a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4052a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4052a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-125">Request body</span></span>
<span data-ttu-id="4052a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4052a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4052a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4052a-127">Response</span></span>
<span data-ttu-id="4052a-128">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4052a-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4052a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4052a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4052a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4052a-130">Request</span></span>
<span data-ttu-id="4052a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4052a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a><span data-ttu-id="4052a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4052a-132">Response</span></span>

<span data-ttu-id="4052a-133">Não há corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4052a-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```http
HTTP/1.1 200 OK
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="4052a-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4052a-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4052a-135">C#</span><span class="sxs-lookup"><span data-stu-id="4052a-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4052a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="4052a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4052a-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4052a-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_synchronizationProfile_pause-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-pause.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
