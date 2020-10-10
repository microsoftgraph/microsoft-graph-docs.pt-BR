---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 848cd382c8133fbfddeefc3eb3951b130a0250e0
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418214"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="5c593-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c593-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="5c593-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c593-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c593-105">Recupere as propriedades e os relacionamentos do objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , que representa a [política de método de autenticação](../resources/authenticationmethodspolicies-overview.md) de entrada de telefone sem senha do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5c593-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="5c593-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="5c593-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="5c593-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="5c593-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c593-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c593-108">Permissions</span></span>
<span data-ttu-id="5c593-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c593-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c593-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c593-111">Permission type</span></span>|<span data-ttu-id="5c593-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c593-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c593-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c593-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c593-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5c593-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5c593-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c593-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c593-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c593-116">Not supported.</span></span>|
|<span data-ttu-id="5c593-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c593-117">Application</span></span>|<span data-ttu-id="5c593-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c593-118">Not supported.</span></span>|

<span data-ttu-id="5c593-119">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="5c593-119">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5c593-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5c593-120">Global admin</span></span>
* <span data-ttu-id="5c593-121">Leitor global</span><span class="sxs-lookup"><span data-stu-id="5c593-121">Global reader</span></span>
* <span data-ttu-id="5c593-122">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="5c593-122">Privileged authentication admin</span></span>
* <span data-ttu-id="5c593-123">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="5c593-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5c593-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c593-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="5c593-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c593-125">Request headers</span></span>
|<span data-ttu-id="5c593-126">Nome</span><span class="sxs-lookup"><span data-stu-id="5c593-126">Name</span></span>|<span data-ttu-id="5c593-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c593-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c593-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c593-128">Authorization</span></span>|<span data-ttu-id="5c593-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c593-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c593-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c593-131">Request body</span></span>
<span data-ttu-id="5c593-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c593-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c593-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c593-133">Response</span></span>

<span data-ttu-id="5c593-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c593-134">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c593-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c593-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c593-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c593-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="5c593-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c593-137">Response</span></span>
<span data-ttu-id="5c593-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c593-138">The following is an example of the response.</span></span>

<span data-ttu-id="5c593-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c593-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

