---
title: Obter emailAuthenticationMethodConfiguration
description: Leia as propriedades e as relações de um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: af941c49671ff5a5a2addc9d8e5877f4922043f2
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469280"
---
# <a name="get-emailauthenticationmethodconfiguration"></a><span data-ttu-id="5e046-103">Obter emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e046-103">Get emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="5e046-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e046-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e046-105">Leia as propriedades e as relações de um [objeto emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) que representa a política de método de autenticação [OTP](../resources/authenticationmethodspolicies-overview.md) de email para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5e046-105">Read the properties and relationships of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e046-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e046-106">Permissions</span></span>

<span data-ttu-id="5e046-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e046-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e046-109">Permission type</span></span>|<span data-ttu-id="5e046-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e046-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e046-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e046-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e046-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5e046-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="5e046-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e046-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e046-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e046-114">Not supported.</span></span>|
|<span data-ttu-id="5e046-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e046-115">Application</span></span>|<span data-ttu-id="5e046-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5e046-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="5e046-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="5e046-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="5e046-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5e046-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5e046-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e046-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfiguration/email
```

## <a name="request-headers"></a><span data-ttu-id="5e046-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e046-120">Request headers</span></span>

|<span data-ttu-id="5e046-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5e046-121">Name</span></span>|<span data-ttu-id="5e046-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e046-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5e046-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e046-123">Authorization</span></span>|<span data-ttu-id="5e046-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e046-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e046-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e046-126">Request body</span></span>

<span data-ttu-id="5e046-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e046-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e046-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e046-128">Response</span></span>

<span data-ttu-id="5e046-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e046-129">If successful, this method returns a `200 OK` response code and an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5e046-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5e046-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5e046-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e046-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethodconfiguration"
}
-->

```http
GET /policies/authenticationMethodsPolicy/email
```

### <a name="response"></a><span data-ttu-id="5e046-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e046-132">Response</span></span>

<span data-ttu-id="5e046-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e046-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "allowExternalIdToUseEmailOtp": "True"
  }
}
```
