---
title: Atualizar autenticaçãoMethodsPolicy
description: Atualize as propriedades de um objeto authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 22630c6651e94faa243e98f275c6d299edd88173
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682859"
---
# <a name="update-authenticationmethodspolicy"></a><span data-ttu-id="d7f83-103">Atualizar autenticaçãoMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="d7f83-103">Update authenticationMethodsPolicy</span></span>
<span data-ttu-id="d7f83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7f83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7f83-105">Atualize as propriedades de [um objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d7f83-105">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7f83-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7f83-106">Permissions</span></span>
<span data-ttu-id="d7f83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7f83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7f83-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7f83-109">Permission type</span></span>|<span data-ttu-id="d7f83-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7f83-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7f83-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7f83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7f83-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d7f83-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="d7f83-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7f83-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7f83-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7f83-114">Not supported.</span></span>|
|<span data-ttu-id="d7f83-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7f83-115">Application</span></span>|<span data-ttu-id="d7f83-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d7f83-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7f83-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7f83-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="d7f83-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7f83-118">Request headers</span></span>
|<span data-ttu-id="d7f83-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d7f83-119">Name</span></span>|<span data-ttu-id="d7f83-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7f83-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d7f83-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7f83-121">Authorization</span></span>|<span data-ttu-id="d7f83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7f83-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d7f83-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7f83-124">Content-Type</span></span>|<span data-ttu-id="d7f83-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7f83-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7f83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7f83-127">Request body</span></span>
<span data-ttu-id="d7f83-128">No corpo da solicitação, fornece uma representação JSON do [objeto registrationEnforcement](../resources/registrationenforcement.md) para solicitar que os usuários configurarem métodos de autenticação direcionados.</span><span class="sxs-lookup"><span data-stu-id="d7f83-128">In the request body, supply a JSON representation of the [registrationEnforcement](../resources/registrationenforcement.md) object to prompt users to set up targeted authentication methods.</span></span> 

|<span data-ttu-id="d7f83-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7f83-129">Property</span></span>|<span data-ttu-id="d7f83-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7f83-130">Type</span></span>|<span data-ttu-id="d7f83-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7f83-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f83-132">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="d7f83-132">registrationEnforcement</span></span>|[<span data-ttu-id="d7f83-133">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="d7f83-133">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="d7f83-134">Impor o registro no momento da inscrição.</span><span class="sxs-lookup"><span data-stu-id="d7f83-134">Enforce registration at sign-in time.</span></span> <span data-ttu-id="d7f83-135">Essa propriedade pode ser usada para solicitar que os usuários configurarem métodos de autenticação direcionados.</span><span class="sxs-lookup"><span data-stu-id="d7f83-135">This property can be used to prompt users to set up targeted authentication methods.</span></span>|

## <a name="response"></a><span data-ttu-id="d7f83-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7f83-136">Response</span></span>
<span data-ttu-id="d7f83-137">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d7f83-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d7f83-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d7f83-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7f83-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7f83-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="d7f83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7f83-140">Response</span></span>
<span data-ttu-id="d7f83-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7f83-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
