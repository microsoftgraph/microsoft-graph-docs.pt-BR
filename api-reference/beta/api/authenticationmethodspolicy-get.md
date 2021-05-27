---
title: Obter authenticationMethodsPolicy
description: Leia as propriedades e as relações de um objeto authenticationMethodsPolicy.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b54b95f3db35d744d400fb50a221cdfdad12890b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682858"
---
# <a name="get-authenticationmethodspolicy"></a><span data-ttu-id="9c58f-103">Obter authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="9c58f-103">Get authenticationMethodsPolicy</span></span>
<span data-ttu-id="9c58f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c58f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c58f-105">Leia as propriedades e as relações de um [objeto authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c58f-105">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c58f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c58f-106">Permissions</span></span>
<span data-ttu-id="9c58f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c58f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c58f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c58f-109">Permission type</span></span>|<span data-ttu-id="9c58f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c58f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c58f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c58f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c58f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c58f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9c58f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c58f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c58f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c58f-114">Not supported.</span></span>|
|<span data-ttu-id="9c58f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c58f-115">Application</span></span>|<span data-ttu-id="9c58f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c58f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c58f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c58f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c58f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c58f-118">Optional query parameters</span></span>
<span data-ttu-id="9c58f-119">Este método não dá suporte a parâmetros de consulta opcionais.</span><span class="sxs-lookup"><span data-stu-id="9c58f-119">This method does not support any optional query parameters.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c58f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c58f-120">Request headers</span></span>
|<span data-ttu-id="9c58f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9c58f-121">Name</span></span>|<span data-ttu-id="9c58f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c58f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c58f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c58f-123">Authorization</span></span>|<span data-ttu-id="9c58f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c58f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c58f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c58f-126">Request body</span></span>
<span data-ttu-id="9c58f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c58f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c58f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c58f-128">Response</span></span>

<span data-ttu-id="9c58f-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c58f-129">If successful, this method returns a `200 OK` response code and an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c58f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c58f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c58f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c58f-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodspolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy
```


### <a name="response"></a><span data-ttu-id="9c58f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c58f-132">Response</span></span>
<span data-ttu-id="9c58f-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c58f-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
