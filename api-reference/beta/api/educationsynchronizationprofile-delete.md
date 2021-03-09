---
title: Excluir um educationSynchronizationProfile
description: Exclua um perfil de sincronização de dados escolares no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2cc7d03b406888022fc8bab935af2b5118357c0c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574276"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="20646-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="20646-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="20646-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20646-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20646-105">Exclua um perfil [de sincronização de](../resources/educationsynchronizationprofile.md) dados escolares no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="20646-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="20646-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20646-106">Permissions</span></span>
<span data-ttu-id="20646-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20646-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20646-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20646-109">Permission type</span></span> | <span data-ttu-id="20646-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="20646-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="20646-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20646-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20646-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20646-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="20646-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20646-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20646-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20646-114">Request headers</span></span>
| <span data-ttu-id="20646-115">Nome</span><span class="sxs-lookup"><span data-stu-id="20646-115">Name</span></span>       | <span data-ttu-id="20646-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="20646-116">Type</span></span> | <span data-ttu-id="20646-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="20646-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20646-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="20646-118">Authorization</span></span>  | <span data-ttu-id="20646-119">string</span><span class="sxs-lookup"><span data-stu-id="20646-119">string</span></span>  | <span data-ttu-id="20646-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20646-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="20646-122">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="20646-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="20646-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20646-123">Not supported.</span></span>|
|<span data-ttu-id="20646-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20646-124">Application</span></span>|<span data-ttu-id="20646-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20646-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20646-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20646-126">Request body</span></span>
<span data-ttu-id="20646-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20646-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="20646-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="20646-128">Response</span></span>
<span data-ttu-id="20646-129">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20646-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="20646-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20646-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20646-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20646-131">Request</span></span>
<span data-ttu-id="20646-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20646-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20646-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="20646-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="20646-134">C#</span><span class="sxs-lookup"><span data-stu-id="20646-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20646-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20646-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20646-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20646-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20646-137">Java</span><span class="sxs-lookup"><span data-stu-id="20646-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20646-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="20646-138">Response</span></span>
<span data-ttu-id="20646-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20646-139">Here is an example of the response.</span></span>
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


