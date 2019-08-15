---
title: Excluir um educationSynchronizationProfile
description: Excluir um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2230d8bc88bfdba6f014c9b78cbdc7f519f075d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416006"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="4e172-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4e172-103">Delete a educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e172-104">Excluir um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="4e172-104">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e172-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e172-105">Permissions</span></span>
<span data-ttu-id="4e172-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e172-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e172-108">Permission type</span></span> | <span data-ttu-id="4e172-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e172-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4e172-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e172-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e172-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e172-111">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e172-112">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e172-112">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4e172-113">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e172-113">Request headers</span></span>
| <span data-ttu-id="4e172-114">Nome</span><span class="sxs-lookup"><span data-stu-id="4e172-114">Name</span></span>       | <span data-ttu-id="4e172-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e172-115">Type</span></span> | <span data-ttu-id="4e172-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e172-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4e172-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e172-117">Authorization</span></span>  | <span data-ttu-id="4e172-118">string</span><span class="sxs-lookup"><span data-stu-id="4e172-118">string</span></span>  | <span data-ttu-id="4e172-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e172-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="4e172-121">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4e172-121">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4e172-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e172-122">Not supported.</span></span>|
|<span data-ttu-id="4e172-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e172-123">Application</span></span>|<span data-ttu-id="4e172-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e172-124">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e172-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e172-125">Request body</span></span>
<span data-ttu-id="4e172-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e172-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e172-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e172-127">Response</span></span>
<span data-ttu-id="4e172-128">Se tiver êxito, este método retornará `202 Accepted` um código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e172-128">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e172-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e172-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e172-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e172-130">Request</span></span>
<span data-ttu-id="4e172-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e172-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e172-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e172-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e172-133">C#</span><span class="sxs-lookup"><span data-stu-id="4e172-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e172-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e172-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e172-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4e172-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4e172-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e172-136">Response</span></span>
<span data-ttu-id="4e172-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e172-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
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
