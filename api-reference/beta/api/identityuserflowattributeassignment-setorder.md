---
title: 'identityUserFlowAttributeAssignment: SetOrder'
description: Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc1487246f5a3370ce1b88f50eafcce7029baf4f
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752729"
---
# <a name="identityuserflowattributeassignment-setorder"></a><span data-ttu-id="56413-103">identityUserFlowAttributeAssignment: SetOrder</span><span class="sxs-lookup"><span data-stu-id="56413-103">identityUserFlowAttributeAssignment: setOrder</span></span>

<span data-ttu-id="56413-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56413-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56413-105">Definir a ordem de identityUserFlowAttributeAssignments que está sendo coletada dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="56413-105">Set the order of identityUserFlowAttributeAssignments being collected within a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="56413-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="56413-106">Permissions</span></span>

<span data-ttu-id="56413-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56413-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56413-109">Permission type</span></span>|<span data-ttu-id="56413-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56413-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56413-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56413-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56413-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56413-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="56413-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56413-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56413-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="56413-114">Not supported</span></span>|
|<span data-ttu-id="56413-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56413-115">Application</span></span>|<span data-ttu-id="56413-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56413-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56413-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56413-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a><span data-ttu-id="56413-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56413-118">Request headers</span></span>

|<span data-ttu-id="56413-119">Nome</span><span class="sxs-lookup"><span data-stu-id="56413-119">Name</span></span>|<span data-ttu-id="56413-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="56413-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="56413-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="56413-121">Authorization</span></span>|<span data-ttu-id="56413-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56413-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="56413-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56413-124">Content-Type</span></span>|<span data-ttu-id="56413-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56413-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56413-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56413-127">Request body</span></span>

<span data-ttu-id="56413-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="56413-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56413-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="56413-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56413-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56413-130">Parameter</span></span>|<span data-ttu-id="56413-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56413-131">Type</span></span>|<span data-ttu-id="56413-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56413-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56413-133">newAssignmentOrder</span><span class="sxs-lookup"><span data-stu-id="56413-133">newAssignmentOrder</span></span>|[<span data-ttu-id="56413-134">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="56413-134">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="56413-135">Usado para definir a ordem dos atributos que estão sendo coletados dentro de um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="56413-135">Used to define the order of the attributes being collected within a user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="56413-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="56413-136">Response</span></span>

<span data-ttu-id="56413-137">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56413-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56413-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56413-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56413-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56413-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="56413-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="56413-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder
Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="56413-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56413-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityuserflowattributeassignment-setorder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="56413-142">C#</span><span class="sxs-lookup"><span data-stu-id="56413-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityuserflowattributeassignment-setorder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56413-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56413-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityuserflowattributeassignment-setorder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56413-144">Java</span><span class="sxs-lookup"><span data-stu-id="56413-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityuserflowattributeassignment-setorder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56413-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="56413-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
