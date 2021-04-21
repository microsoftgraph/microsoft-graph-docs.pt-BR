---
title: Excluir userAttributeAssignment
description: Exclua um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8dab44862a1859851a4c3fb9b52dcd8f3692e8c1
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920766"
---
# <a name="delete-userattributeassignment"></a><span data-ttu-id="96825-103">Excluir userAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="96825-103">Delete userAttributeAssignment</span></span>

<span data-ttu-id="96825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96825-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96825-105">[Exclua um objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="96825-105">Delete an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96825-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96825-106">Permissions</span></span>

<span data-ttu-id="96825-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96825-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96825-109">Permission type</span></span>|<span data-ttu-id="96825-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96825-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96825-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96825-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96825-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96825-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="96825-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96825-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96825-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="96825-114">Not supported</span></span>|
|<span data-ttu-id="96825-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96825-115">Application</span></span>|<span data-ttu-id="96825-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96825-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96825-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96825-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-118">Request headers</span></span>

|<span data-ttu-id="96825-119">Nome</span><span class="sxs-lookup"><span data-stu-id="96825-119">Name</span></span>|<span data-ttu-id="96825-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="96825-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96825-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96825-121">Authorization</span></span>|<span data-ttu-id="96825-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96825-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96825-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-124">Request body</span></span>

<span data-ttu-id="96825-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96825-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96825-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-126">Response</span></span>

<span data-ttu-id="96825-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="96825-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="96825-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96825-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96825-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96825-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userattributeassignments_from_b2xidentityuserflow"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```
# <a name="c"></a>[<span data-ttu-id="96825-131">C#</span><span class="sxs-lookup"><span data-stu-id="96825-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userattributeassignments-from-b2xidentityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96825-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96825-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userattributeassignments-from-b2xidentityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96825-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96825-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userattributeassignments-from-b2xidentityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96825-134">Java</span><span class="sxs-lookup"><span data-stu-id="96825-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userattributeassignments-from-b2xidentityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96825-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
