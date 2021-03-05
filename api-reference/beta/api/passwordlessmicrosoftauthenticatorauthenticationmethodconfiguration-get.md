---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2c6ce5a53c5be64f0cb7319a390b3ad8c0d3fead
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472059"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="1709a-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (preterido)</span><span class="sxs-lookup"><span data-stu-id="1709a-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="1709a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1709a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1709a-105">Recupere as propriedades e as relações do [objetoMicrosoftAuthenticatorAuthenticationAuthenticationMethodConfiguration,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) que representa [](../resources/authenticationmethodspolicies-overview.md) a política de autenticação de autenticação de telefone sem senha do Microsoft Authenticator Passwordless Phone Sign-in para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1709a-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="1709a-106">A API de política de autenticação do método de autenticação de telefone sem senha do Microsoft Authenticator é preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="1709a-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="1709a-107">Use a nova política de método de autenticação do [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1709a-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1709a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1709a-108">Permissions</span></span>
<span data-ttu-id="1709a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1709a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1709a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1709a-111">Permission type</span></span>|<span data-ttu-id="1709a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1709a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1709a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1709a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1709a-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1709a-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1709a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1709a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1709a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1709a-116">Not supported.</span></span>|
|<span data-ttu-id="1709a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1709a-117">Application</span></span>|<span data-ttu-id="1709a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1709a-118">Not supported.</span></span>|

<span data-ttu-id="1709a-119">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1709a-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1709a-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1709a-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="1709a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1709a-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="1709a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1709a-122">Request headers</span></span>
|<span data-ttu-id="1709a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1709a-123">Name</span></span>|<span data-ttu-id="1709a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1709a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1709a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1709a-125">Authorization</span></span>|<span data-ttu-id="1709a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1709a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1709a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1709a-128">Request body</span></span>
<span data-ttu-id="1709a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1709a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1709a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1709a-130">Response</span></span>

<span data-ttu-id="1709a-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1709a-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1709a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1709a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1709a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1709a-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1709a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1709a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```
# <a name="c"></a>[<span data-ttu-id="1709a-135">C#</span><span class="sxs-lookup"><span data-stu-id="1709a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1709a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1709a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1709a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1709a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1709a-138">Java</span><span class="sxs-lookup"><span data-stu-id="1709a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1709a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1709a-139">Response</span></span>
<span data-ttu-id="1709a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1709a-140">The following is an example of the response.</span></span>

<span data-ttu-id="1709a-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1709a-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

