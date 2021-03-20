---
title: Obter microsoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f94c20bcfb29de6af6ec77371594b367ed93e88b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948960"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="ac557-103">Obter microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac557-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="ac557-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac557-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac557-105">Recupere as propriedades e as relações do [objeto microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) que representa a política de método de autenticação do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac557-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac557-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac557-106">Permissions</span></span>
<span data-ttu-id="ac557-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac557-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac557-109">Permission type</span></span>|<span data-ttu-id="ac557-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac557-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac557-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac557-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac557-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ac557-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="ac557-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac557-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac557-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac557-114">Not supported.</span></span>|
|<span data-ttu-id="ac557-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac557-115">Application</span></span>|<span data-ttu-id="ac557-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ac557-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="ac557-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="ac557-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="ac557-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="ac557-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="ac557-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac557-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="ac557-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac557-120">Request headers</span></span>
|<span data-ttu-id="ac557-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ac557-121">Name</span></span>|<span data-ttu-id="ac557-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac557-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac557-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac557-123">Authorization</span></span>|<span data-ttu-id="ac557-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac557-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac557-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac557-126">Request body</span></span>
<span data-ttu-id="ac557-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac557-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac557-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac557-128">Response</span></span>

<span data-ttu-id="ac557-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac557-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac557-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ac557-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac557-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac557-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="ac557-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac557-132">Response</span></span>
<span data-ttu-id="ac557-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ac557-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
    "id": "129ae788-e788-129a-88e7-9a1288e79a12",
    "state": "String"
  }
}
```

