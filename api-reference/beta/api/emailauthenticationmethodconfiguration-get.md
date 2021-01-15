---
title: Obter emailAuthenticationMethodConfiguration
description: Leia as propriedades e os relacionamentos de um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82f1653e5fdf091bd92638b4596bacd4b8194817
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873322"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="5743b-103">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5743b-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="5743b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5743b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5743b-105">Leia as propriedades e as relações de um objeto [emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) que representa a política de método de autenticação [OTP](../resources/authenticationmethodspolicies-overview.md) de email para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5743b-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5743b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5743b-106">Permissions</span></span>

<span data-ttu-id="5743b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5743b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5743b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5743b-109">Permission type</span></span>|<span data-ttu-id="5743b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5743b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5743b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5743b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5743b-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5743b-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5743b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5743b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5743b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5743b-114">Not supported.</span></span>|
|<span data-ttu-id="5743b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5743b-115">Application</span></span>|<span data-ttu-id="5743b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5743b-116">Not supported.</span></span>|

<span data-ttu-id="5743b-117">Para cenários delegados, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5743b-117">For delegated scenarios the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5743b-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5743b-118">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5743b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5743b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="5743b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5743b-120">Request headers</span></span>

|<span data-ttu-id="5743b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5743b-121">Name</span></span>|<span data-ttu-id="5743b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5743b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5743b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5743b-123">Authorization</span></span>|<span data-ttu-id="5743b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5743b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5743b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5743b-126">Request body</span></span>

<span data-ttu-id="5743b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5743b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5743b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5743b-128">Response</span></span>

<span data-ttu-id="5743b-129">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5743b-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5743b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5743b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5743b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5743b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="5743b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5743b-132">Response</span></span>

<span data-ttu-id="5743b-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5743b-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 491

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
    "id": "Email",
    "state": "enabled",
    "allowExternalIdToUseEmailOtp": "True",
    "includeTargets":[
        {
          "targetType":"group",
          "id":"all_users",
          "isRegistrationRequired":false,
        }
    ]
  }
}
```

