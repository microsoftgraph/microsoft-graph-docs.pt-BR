---
title: Excluir userAttributeAssignment
description: Exclua um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9c4e54cdc248e88833d50d89ef6051925d3391db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435144"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="2d742-103">Excluir userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="2d742-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="2d742-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d742-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d742-105">[Exclua um objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2d742-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d742-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d742-106">Permissions</span></span>

<span data-ttu-id="2d742-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d742-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d742-109">Permission type</span></span>|<span data-ttu-id="2d742-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d742-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d742-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d742-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d742-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d742-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2d742-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d742-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d742-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2d742-114">Not supported</span></span>|
|<span data-ttu-id="2d742-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d742-115">Application</span></span>|<span data-ttu-id="2d742-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d742-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d742-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d742-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2d742-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d742-118">Request headers</span></span>

|<span data-ttu-id="2d742-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2d742-119">Name</span></span>|<span data-ttu-id="2d742-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d742-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d742-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d742-121">Authorization</span></span>|<span data-ttu-id="2d742-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d742-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d742-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d742-124">Request body</span></span>

<span data-ttu-id="2d742-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d742-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d742-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d742-126">Response</span></span>

<span data-ttu-id="2d742-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d742-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2d742-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2d742-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d742-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d742-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2d742-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d742-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2cidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="2d742-131">C#</span><span class="sxs-lookup"><span data-stu-id="2d742-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2cidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d742-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d742-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2cidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d742-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d742-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2cidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d742-134">Java</span><span class="sxs-lookup"><span data-stu-id="2d742-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2cidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d742-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d742-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
