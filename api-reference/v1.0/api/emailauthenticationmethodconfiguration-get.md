---
title: Obter emailAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 54bc1d89730590a01bf7787d20313279067eb27a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231994"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="41097-103">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="41097-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="41097-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41097-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41097-105">Leia as propriedades e as relações de um [objeto emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) que representa a política de método de autenticação [OTP](../resources/authenticationmethodspolicies-overview.md) de email para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="41097-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="41097-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41097-106">Permissions</span></span>

<span data-ttu-id="41097-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41097-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41097-109">Permission type</span></span>|<span data-ttu-id="41097-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41097-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41097-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41097-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41097-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="41097-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="41097-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41097-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41097-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41097-114">Not supported.</span></span>|
|<span data-ttu-id="41097-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41097-115">Application</span></span>|<span data-ttu-id="41097-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="41097-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="41097-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="41097-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="41097-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="41097-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="41097-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41097-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="41097-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41097-120">Request headers</span></span>

|<span data-ttu-id="41097-121">Nome</span><span class="sxs-lookup"><span data-stu-id="41097-121">Name</span></span>|<span data-ttu-id="41097-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="41097-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="41097-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="41097-123">Authorization</span></span>|<span data-ttu-id="41097-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41097-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41097-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41097-126">Request body</span></span>

<span data-ttu-id="41097-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41097-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41097-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="41097-128">Response</span></span>

<span data-ttu-id="41097-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41097-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41097-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41097-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41097-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41097-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="41097-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="41097-132">Response</span></span>

<span data-ttu-id="41097-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="41097-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "allowExternalIdToUseEmailOtp": "enabled"
  }
}
```
