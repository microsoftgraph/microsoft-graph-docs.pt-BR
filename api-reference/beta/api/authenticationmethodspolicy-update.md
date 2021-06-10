---
title: Atualizar autenticaçãoMethodsPolicy
description: Atualize as propriedades de um objeto authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: cc9c67d5f01d45b1231d1d92922c45c02b3515f4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869077"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="ed0f0-103">Atualizar autenticaçãoMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="ed0f0-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="ed0f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed0f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed0f0-105">Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ed0f0-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed0f0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ed0f0-106">Permissions</span></span>
<span data-ttu-id="ed0f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed0f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed0f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed0f0-109">Permission type</span></span>|<span data-ttu-id="ed0f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed0f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed0f0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed0f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed0f0-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed0f0-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="ed0f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed0f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed0f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-114">Not supported.</span></span>|
|<span data-ttu-id="ed0f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed0f0-115">Application</span></span>|<span data-ttu-id="ed0f0-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ed0f0-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed0f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed0f0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="ed0f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0f0-118">Request headers</span></span>
|<span data-ttu-id="ed0f0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed0f0-119">Name</span></span>|<span data-ttu-id="ed0f0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed0f0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed0f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed0f0-121">Authorization</span></span>|<span data-ttu-id="ed0f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ed0f0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed0f0-124">Content-Type</span></span>|<span data-ttu-id="ed0f0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed0f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0f0-127">Request body</span></span>
<span data-ttu-id="ed0f0-128">No corpo da solicitação, fornece uma representação JSON do [objeto registrationEnforcement](../resources/registrationenforcement.md) para solicitar que os usuários configurarem métodos de autenticação direcionados.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="ed0f0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed0f0-129">Property</span></span>|<span data-ttu-id="ed0f0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed0f0-130">Type</span></span>|<span data-ttu-id="ed0f0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed0f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed0f0-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="ed0f0-132">registrationEnforcement</span></span>|[<span data-ttu-id="ed0f0-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="ed0f0-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="ed0f0-134">Impor o registro no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="ed0f0-135">Essa propriedade pode ser usada para solicitar que os usuários configurarem métodos de autenticação direcionados.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="ed0f0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0f0-136">Response</span></span>
<span data-ttu-id="ed0f0-137">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ed0f0-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed0f0-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed0f0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0f0-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed0f0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed0f0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodspolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
Content-Type: application/json
Content-length: 293

{
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
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
# <a name="c"></a>[<span data-ttu-id="ed0f0-141">C#</span><span class="sxs-lookup"><span data-stu-id="ed0f0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed0f0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed0f0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed0f0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed0f0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed0f0-144">Java</span><span class="sxs-lookup"><span data-stu-id="ed0f0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ed0f0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0f0-145">Response</span></span>
<span data-ttu-id="ed0f0-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed0f0-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "lastModifiedDateTime": "2021-05-25T01:08:08.6712279Z",
  "policyVersion": "1.4",
  "registrationEnforcement": {
    "authenticationMethodsRegistrationCampaign": {
        "snoozeDurationInDays": 1,
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
