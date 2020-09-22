---
title: Excluir um educationSynchronizationProfile
description: Excluir um perfil de sincronização de dados da escola no locatário com base no identificador.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39bc4909e63e6e7ff908481873f32324703bf549
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991254"
---
# <a name="delete-a-educationsynchronizationprofile"></a><span data-ttu-id="4f393-103">Excluir um educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4f393-103">Delete a educationSynchronizationProfile</span></span>

<span data-ttu-id="4f393-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f393-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f393-105">Excluir um perfil de [sincronização](../resources/educationsynchronizationprofile.md) de dados da escola no locatário com base no identificador.</span><span class="sxs-lookup"><span data-stu-id="4f393-105">Delete a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f393-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f393-106">Permissions</span></span>
<span data-ttu-id="4f393-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f393-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f393-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f393-109">Permission type</span></span> | <span data-ttu-id="4f393-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f393-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4f393-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f393-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f393-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f393-112">EduAdministration.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f393-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f393-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4f393-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f393-114">Request headers</span></span>
| <span data-ttu-id="4f393-115">Nome</span><span class="sxs-lookup"><span data-stu-id="4f393-115">Name</span></span>       | <span data-ttu-id="4f393-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f393-116">Type</span></span> | <span data-ttu-id="4f393-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f393-117">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f393-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f393-118">Authorization</span></span>  | <span data-ttu-id="4f393-119">string</span><span class="sxs-lookup"><span data-stu-id="4f393-119">string</span></span>  | <span data-ttu-id="4f393-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f393-p102">Bearer {token}. Required.</span></span>  |
|<span data-ttu-id="4f393-122">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4f393-122">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4f393-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f393-123">Not supported.</span></span>|
|<span data-ttu-id="4f393-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f393-124">Application</span></span>|<span data-ttu-id="4f393-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f393-125">Not supported.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f393-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f393-126">Request body</span></span>
<span data-ttu-id="4f393-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f393-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4f393-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f393-128">Response</span></span>
<span data-ttu-id="4f393-129">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f393-129">If successful, this method returns a `202 Accepted` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f393-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f393-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f393-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f393-131">Request</span></span>
<span data-ttu-id="4f393-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f393-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f393-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f393-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationProfile"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="4f393-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f393-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f393-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f393-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f393-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f393-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f393-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f393-137">Response</span></span>
<span data-ttu-id="4f393-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f393-138">Here is an example of the response.</span></span>
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


