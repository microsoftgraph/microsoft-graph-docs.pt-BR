---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e47045c6eb34c393cffb89d004fb1c7a27efc49d
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086757"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="eb176-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb176-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="eb176-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb176-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb176-105">Recupere as propriedades e os relacionamentos do objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , que representa a [política de método de autenticação](../resources/authenticationmethodspolicies-overview.md) de entrada de telefone sem senha do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eb176-105">Retrieve the properties and relationships of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="eb176-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="eb176-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="eb176-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="eb176-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb176-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb176-108">Permissions</span></span>
<span data-ttu-id="eb176-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb176-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb176-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb176-111">Permission type</span></span>|<span data-ttu-id="eb176-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb176-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb176-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb176-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb176-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="eb176-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="eb176-115">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="eb176-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb176-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb176-116">Not supported.</span></span>|
|<span data-ttu-id="eb176-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb176-117">Application</span></span>|<span data-ttu-id="eb176-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb176-118">Not supported.</span></span>|

<span data-ttu-id="eb176-119">Para cenários delegados, o administrador precisa da seguinte [função](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="eb176-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="eb176-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="eb176-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="eb176-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb176-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="eb176-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb176-122">Request headers</span></span>
|<span data-ttu-id="eb176-123">Nome</span><span class="sxs-lookup"><span data-stu-id="eb176-123">Name</span></span>|<span data-ttu-id="eb176-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb176-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb176-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb176-125">Authorization</span></span>|<span data-ttu-id="eb176-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb176-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb176-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb176-128">Request body</span></span>
<span data-ttu-id="eb176-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb176-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb176-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb176-130">Response</span></span>

<span data-ttu-id="eb176-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb176-131">If successful, this method returns a `200 OK` response code and a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb176-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb176-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb176-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb176-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="eb176-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb176-134">Response</span></span>
<span data-ttu-id="eb176-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb176-135">The following is an example of the response.</span></span>

<span data-ttu-id="eb176-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb176-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

