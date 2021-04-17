---
title: Obter authenticationFlowsPolicy
description: Ler as propriedades e relações de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7f96ffc150ef5ac2eefc759059e163560a6c8841
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882859"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="c6b07-103">Obter authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="c6b07-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="c6b07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6b07-105">Ler as propriedades e relações de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c6b07-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6b07-106">Permissions</span></span>

<span data-ttu-id="c6b07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6b07-109">Permission type</span></span>|<span data-ttu-id="c6b07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6b07-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6b07-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6b07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c6b07-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="c6b07-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="c6b07-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6b07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6b07-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="c6b07-114">Not Supported</span></span>|
|<span data-ttu-id="c6b07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6b07-115">Application</span></span>|<span data-ttu-id="c6b07-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="c6b07-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6b07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6b07-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="c6b07-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b07-118">Request headers</span></span>

|<span data-ttu-id="c6b07-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6b07-119">Name</span></span>|<span data-ttu-id="c6b07-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6b07-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c6b07-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6b07-121">Authorization</span></span>|<span data-ttu-id="c6b07-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6b07-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6b07-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b07-124">Request body</span></span>

<span data-ttu-id="c6b07-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6b07-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6b07-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b07-126">Response</span></span>

<span data-ttu-id="c6b07-127">Se bem-sucedido, este método retorna um `200 OK`código de resposta e um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6b07-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6b07-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6b07-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c6b07-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b07-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
```

### <a name="response"></a><span data-ttu-id="c6b07-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b07-130">Response</span></span>

<span data-ttu-id="c6b07-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6b07-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authenticationFlowsPolicy/$entity",
    "id": "authenticationFlowsPolicy",
    "displayName": "Authentication flows policy",
    "description": "Authentication flows policy allows modification of settings related to authentication flows in AAD tenant, such as self-service sign up configuration.",
    "selfServiceSignUp": {
        "isEnabled": true
    }
}
```
