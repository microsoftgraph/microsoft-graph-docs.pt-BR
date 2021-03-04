---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c21d1c8601715beef6f056defbf203afa417ac0c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447756"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="9c53d-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (preterido)</span><span class="sxs-lookup"><span data-stu-id="9c53d-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="9c53d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c53d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c53d-105">Recupere as propriedades e as relações do [objetoMicrosoftAuthenticatorAuthenticationAuthenticationMethodConfiguration,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) que representa [](../resources/authenticationmethodspolicies-overview.md) a política de autenticação de autenticação de telefone sem senha do Microsoft Authenticator Passwordless Phone Sign-in para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c53d-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="9c53d-106">A API de política de autenticação do método de autenticação de telefone sem senha do Microsoft Authenticator é preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="9c53d-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="9c53d-107">Use a nova política de método de autenticação do [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c53d-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c53d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c53d-108">Permissions</span></span>
<span data-ttu-id="9c53d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c53d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c53d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c53d-111">Permission type</span></span>|<span data-ttu-id="9c53d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c53d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c53d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c53d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c53d-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c53d-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9c53d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c53d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c53d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c53d-116">Not supported.</span></span>|
|<span data-ttu-id="9c53d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c53d-117">Application</span></span>|<span data-ttu-id="9c53d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c53d-118">Not supported.</span></span>|

<span data-ttu-id="9c53d-119">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9c53d-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9c53d-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9c53d-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="9c53d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c53d-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="9c53d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c53d-122">Request headers</span></span>
|<span data-ttu-id="9c53d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9c53d-123">Name</span></span>|<span data-ttu-id="9c53d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c53d-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c53d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c53d-125">Authorization</span></span>|<span data-ttu-id="9c53d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c53d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c53d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c53d-128">Request body</span></span>
<span data-ttu-id="9c53d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c53d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c53d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c53d-130">Response</span></span>

<span data-ttu-id="9c53d-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c53d-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c53d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9c53d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c53d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c53d-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="9c53d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c53d-134">Response</span></span>
<span data-ttu-id="9c53d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c53d-135">The following is an example of the response.</span></span>

<span data-ttu-id="9c53d-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c53d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "PasswordlessMicrosoftAuthenticator",
    "state": "enabled",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}
```

