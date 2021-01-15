---
title: Obter microsoftAuthenticatorAuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8eb1862fc301edb154d334f62cd82958abb39071
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874468"
---
# <a name="get-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="e36f3-103">Obter microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="e36f3-103">Get microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="e36f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e36f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e36f3-105">Recupere as propriedades e as relações do objeto [microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) que representa a política de método de autenticação do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e36f3-105">Retrieve the properties and relationships of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e36f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e36f3-106">Permissions</span></span>
<span data-ttu-id="e36f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e36f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e36f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e36f3-109">Permission type</span></span>|<span data-ttu-id="e36f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e36f3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e36f3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e36f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e36f3-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e36f3-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="e36f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e36f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e36f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e36f3-114">Not supported.</span></span>|
|<span data-ttu-id="e36f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e36f3-115">Application</span></span>|<span data-ttu-id="e36f3-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e36f3-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="e36f3-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="e36f3-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="e36f3-118">Para obter mais informações, consulte [a função.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e36f3-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="e36f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e36f3-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="e36f3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e36f3-120">Request headers</span></span>
|<span data-ttu-id="e36f3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e36f3-121">Name</span></span>|<span data-ttu-id="e36f3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e36f3-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e36f3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e36f3-123">Authorization</span></span>|<span data-ttu-id="e36f3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e36f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e36f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e36f3-126">Request body</span></span>
<span data-ttu-id="e36f3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e36f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e36f3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e36f3-128">Response</span></span>

<span data-ttu-id="e36f3-129">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e36f3-129">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e36f3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e36f3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e36f3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e36f3-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```


### <a name="response"></a><span data-ttu-id="e36f3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e36f3-132">Response</span></span>
<span data-ttu-id="e36f3-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e36f3-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

