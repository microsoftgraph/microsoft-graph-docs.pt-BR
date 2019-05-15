---
title: Excluir um educationSynchronizationProfile
description: Excluir um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 347efaf51f258535c1217252f4df5a22091fa7ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960862"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="37523-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="37523-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37523-104">Excluir um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="37523-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="37523-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37523-105">Permissions</span></span>
<span data-ttu-id="37523-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37523-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37523-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37523-108">Permission type</span></span> | <span data-ttu-id="37523-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="37523-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="37523-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37523-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37523-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37523-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37523-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37523-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="37523-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37523-113">Request headers</span></span>
| <span data-ttu-id="37523-114">Nome</span><span class="sxs-lookup"><span data-stu-id="37523-114">Name</span></span>       | <span data-ttu-id="37523-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="37523-115">Type</span></span> | <span data-ttu-id="37523-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="37523-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="37523-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="37523-117">Authorization</span></span>  | <span data-ttu-id="37523-118">string</span><span class="sxs-lookup"><span data-stu-id="37523-118">string</span></span>  | <span data-ttu-id="37523-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37523-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="37523-121">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="37523-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="37523-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37523-122">Not supported.</span></span>|
|<span data-ttu-id="37523-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37523-123">Application</span></span>|<span data-ttu-id="37523-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37523-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37523-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37523-125">Request body</span></span>
<span data-ttu-id="37523-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37523-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="37523-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="37523-127">Response</span></span>
<span data-ttu-id="37523-128">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37523-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="37523-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37523-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37523-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37523-130">Request</span></span>
<span data-ttu-id="37523-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37523-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="37523-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37523-132">Response</span></span>
<span data-ttu-id="37523-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37523-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="37523-134">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="37523-134">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37523-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="37523-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="37523-136">C#</span><span class="sxs-lookup"><span data-stu-id="37523-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationProfile-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
