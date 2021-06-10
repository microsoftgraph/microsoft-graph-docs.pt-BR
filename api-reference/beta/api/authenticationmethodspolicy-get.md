---
title: Obter authenticationMethodsPolicy
description: Leia as propriedades e as relações de um objeto authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8c4e737187726f45bb546ea16d09d3ce476401fa
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869474"
---
# <a name="get-authenticationmethodspolicy"></a><span data-ttu-id="dfa37-103">Obter authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="dfa37-103">Get authenticationMethodsPolicy</span></span>
<span data-ttu-id="dfa37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfa37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa37-105">Leia as propriedades e as relações de um [objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dfa37-105">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa37-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dfa37-106">Permissions</span></span>
<span data-ttu-id="dfa37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa37-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfa37-109">Permission type</span></span>|<span data-ttu-id="dfa37-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfa37-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfa37-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfa37-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dfa37-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dfa37-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="dfa37-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfa37-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfa37-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfa37-114">Not supported.</span></span>|
|<span data-ttu-id="dfa37-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfa37-115">Application</span></span>|<span data-ttu-id="dfa37-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dfa37-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfa37-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfa37-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfa37-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfa37-118">Optional query parameters</span></span>
<span data-ttu-id="dfa37-119">Este método não dá suporte a parâmetros de consulta opcionais.</span><span class="sxs-lookup"><span data-stu-id="dfa37-119">This method does not support any optional query parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa37-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa37-120">Request headers</span></span>
|<span data-ttu-id="dfa37-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dfa37-121">Name</span></span>|<span data-ttu-id="dfa37-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfa37-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dfa37-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfa37-123">Authorization</span></span>|<span data-ttu-id="dfa37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfa37-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfa37-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa37-126">Request body</span></span>
<span data-ttu-id="dfa37-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfa37-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa37-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfa37-128">Response</span></span>

<span data-ttu-id="dfa37-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfa37-129">If successful, this method returns a `200 OK` response code and an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfa37-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfa37-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfa37-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfa37-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dfa37-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfa37-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```
# <a name="c"></a>[<span data-ttu-id="dfa37-133">C#</span><span class="sxs-lookup"><span data-stu-id="dfa37-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfa37-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfa37-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfa37-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfa37-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfa37-136">Java</span><span class="sxs-lookup"><span data-stu-id="dfa37-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dfa37-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfa37-137">Response</span></span>
<span data-ttu-id="dfa37-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dfa37-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodsPolicy",
    "id": "authenticationMethodsPolicy",
    "displayName": "Authentication Methods Policy",
    "description": "The tenant-wide policy that controls which authentication methods are allowed in the tenant, authentication method registration requirements, and self-service password reset settings",
    "lastModifiedDateTime": "2021-05-24T18:02:30.5288302Z",
    "policyVersion": "1.4",
    "registrationEnforcement": {
        "authenticationMethodsRegistrationCampaign": {
            "snoozeDurationInDays": 2,
            "state": "enabled",
            "excludeTargets": [],
            "includeTargets": [
                {
                    "id": "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
                    "targetType": "group",
                    "targetedAuthenticationMethod": "microsoftAuthenticator"
                }
            ]
        }
    }
}
```
