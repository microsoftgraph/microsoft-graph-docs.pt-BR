---
title: Obter temporaryAccessPassAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b0874968f9cce1b60a3b0f85a68ac4ccbf9a887e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049643"
---
# <a name="get-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="9c6ba-103">Obter temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c6ba-103">Get temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="9c6ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c6ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c6ba-105">Leia as propriedades e as relações de um [objeto temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) que representa a política de método de autenticação Passagem de Acesso Temporário para o locatário do Azure Active Directory (Azure AD). [](../resources/authenticationmethodspolicies-overview.md)</span><span class="sxs-lookup"><span data-stu-id="9c6ba-105">Read the properties and relationships of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object, which represents the Temporary Access Pass [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c6ba-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c6ba-106">Permissions</span></span>
<span data-ttu-id="9c6ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c6ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c6ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c6ba-109">Permission type</span></span>|<span data-ttu-id="9c6ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c6ba-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c6ba-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c6ba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c6ba-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c6ba-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="9c6ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c6ba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c6ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-114">Not supported.</span></span>|
|<span data-ttu-id="9c6ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c6ba-115">Application</span></span>|<span data-ttu-id="9c6ba-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c6ba-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="9c6ba-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="9c6ba-118">Para obter mais informações, consulte[funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="9c6ba-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="9c6ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c6ba-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```
## <a name="request-headers"></a><span data-ttu-id="9c6ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c6ba-120">Request headers</span></span>
|<span data-ttu-id="9c6ba-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9c6ba-121">Name</span></span>|<span data-ttu-id="9c6ba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c6ba-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9c6ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c6ba-123">Authorization</span></span>|<span data-ttu-id="9c6ba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c6ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c6ba-126">Request body</span></span>
<span data-ttu-id="9c6ba-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-127">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="9c6ba-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c6ba-128">Response</span></span>
<span data-ttu-id="9c6ba-129">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-129">The following is an example of the response.</span></span>

<span data-ttu-id="9c6ba-130">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c6ba-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#authenticationMethodConfigurations/$entity",
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
    "id": "TemporaryAccessPass",
    "state": "enabled",
    "defaultLifetimeInMinutes": 60,
    "defaultLength": 12,
    "minimumLifetimeInMinutes": 60,
    "maximumLifetimeInMinutes": 1440,
    "isUsableOnce": false,
    "includeTargets@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authenticationMethodsPolicy/authenticationMethodConfigurations('TemporaryAccessPass')/microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration/includeTargets",
    "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false
        }
    ]
}
```