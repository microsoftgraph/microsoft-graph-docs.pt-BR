---
title: Obter authenticationFlowsPolicy
description: Leia as propriedades e os relacionamentos de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 843eb458788200a4e2fe6e0248f6966090abe1f0
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556371"
---
# <a name="get-authenticationflowspolicy"></a><span data-ttu-id="d32b3-103">Obter authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="d32b3-103">Get authenticationFlowsPolicy</span></span>

<span data-ttu-id="d32b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d32b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d32b3-105">Leia as propriedades e os relacionamentos de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d32b3-105">Read the properties and relationships of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d32b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d32b3-106">Permissions</span></span>
<span data-ttu-id="d32b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d32b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d32b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d32b3-109">Permission type</span></span>|<span data-ttu-id="d32b3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d32b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d32b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d32b3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d32b3-112">Policy. Read. All, Policy. ReadWrite. AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="d32b3-112">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="d32b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d32b3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d32b3-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d32b3-114">Not Supported</span></span>|
|<span data-ttu-id="d32b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d32b3-115">Application</span></span>|<span data-ttu-id="d32b3-116">Policy. Read. All, Policy. ReadWrite. AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="d32b3-116">Policy.Read.All, Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="d32b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d32b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="d32b3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d32b3-118">Request headers</span></span>
|<span data-ttu-id="d32b3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d32b3-119">Name</span></span>|<span data-ttu-id="d32b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d32b3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d32b3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d32b3-121">Authorization</span></span>|<span data-ttu-id="d32b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d32b3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d32b3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d32b3-124">Request body</span></span>
<span data-ttu-id="d32b3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d32b3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d32b3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d32b3-126">Response</span></span>

<span data-ttu-id="d32b3-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d32b3-127">If successful, this method returns a `200 OK` response code and an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d32b3-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d32b3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d32b3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d32b3-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_authenticationflowspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

### <a name="response"></a><span data-ttu-id="d32b3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d32b3-130">Response</span></span>
<span data-ttu-id="d32b3-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d32b3-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
