---
title: Obter authenticationFlowsPolicy
description: Ler as propriedades e relações de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9d90eab2779baa0626ec660bf41c5af16f52bbce
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872433"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="fe301-103">Obter authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="fe301-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="fe301-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe301-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe301-105">Ler as propriedades e relações de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fe301-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe301-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe301-106">Permissions</span></span>
<span data-ttu-id="fe301-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe301-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe301-109">Permission type</span></span>|<span data-ttu-id="fe301-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe301-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe301-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe301-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe301-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="fe301-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="fe301-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe301-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe301-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="fe301-114">Not Supported</span></span>|
|<span data-ttu-id="fe301-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe301-115">Application</span></span>|<span data-ttu-id="fe301-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="fe301-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe301-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe301-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="fe301-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe301-118">Request headers</span></span>
|<span data-ttu-id="fe301-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fe301-119">Name</span></span>|<span data-ttu-id="fe301-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe301-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fe301-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe301-121">Authorization</span></span>|<span data-ttu-id="fe301-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe301-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe301-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe301-124">Request body</span></span>
<span data-ttu-id="fe301-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe301-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe301-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe301-126">Response</span></span>

<span data-ttu-id="fe301-127">Se bem-sucedido, este método retorna um `200 OK`código de resposta e um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe301-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe301-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe301-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe301-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe301-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fe301-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe301-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```
# <a name="c"></a>[<span data-ttu-id="fe301-131">C#</span><span class="sxs-lookup"><span data-stu-id="fe301-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe301-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe301-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe301-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe301-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe301-134">Java</span><span class="sxs-lookup"><span data-stu-id="fe301-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe301-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe301-135">Response</span></span>
<span data-ttu-id="fe301-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fe301-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationFlowsPolicy"
}
-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationFlowsPolicy/$entity",
    "id": "authenticationFlowsPolicy",
    "displayName": "Authentication flows policy",
    "description": "Authentication flows policy allows modification of settings related to authentication flows in AAD tenant, such as self-service sign up configuration.",
    "selfServiceSignUp": {
        "isEnabled": true
    }
}
```


