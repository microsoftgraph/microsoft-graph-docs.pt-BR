---
title: Atualizar emailAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto emailAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e4091cebd425fb75c11587ca9c02cf68e7b38d6c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351269"
---
# <a name="update-emailauthenticationmethodconfiguration"></a><span data-ttu-id="aec2f-103">Atualizar emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="aec2f-103">Update emailAuthenticationMethodConfiguration</span></span>

<span data-ttu-id="aec2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aec2f-105">Atualize as propriedades de um [objeto emailAuthenticationMethodConfiguration,](../resources/emailauthenticationmethodconfiguration.md) que representa a política de método de autenticação [OTP](../resources/authenticationmethodspolicies-overview.md) de email para o locatário do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="aec2f-105">Update the properties of an [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object, which represents the email OTP [authentication method policy](../resources/authenticationmethodspolicies-overview.md) for the Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="aec2f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aec2f-106">Permissions</span></span>
<span data-ttu-id="aec2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aec2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aec2f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aec2f-109">Permission type</span></span>|<span data-ttu-id="aec2f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aec2f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aec2f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aec2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aec2f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aec2f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="aec2f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aec2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aec2f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aec2f-114">Not supported.</span></span>|
|<span data-ttu-id="aec2f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aec2f-115">Application</span></span>|<span data-ttu-id="aec2f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aec2f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="aec2f-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="aec2f-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="aec2f-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="aec2f-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="aec2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aec2f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
```

## <a name="request-headers"></a><span data-ttu-id="aec2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aec2f-120">Request headers</span></span>

|<span data-ttu-id="aec2f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="aec2f-121">Name</span></span>|<span data-ttu-id="aec2f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aec2f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aec2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aec2f-123">Authorization</span></span>|<span data-ttu-id="aec2f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aec2f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aec2f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aec2f-126">Content-Type</span></span>|<span data-ttu-id="aec2f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aec2f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aec2f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aec2f-129">Request body</span></span>

<span data-ttu-id="aec2f-130">No corpo da solicitação, fornece uma representação JSON do [objeto emailAuthenticationMethodConfiguration.](../resources/emailauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aec2f-130">In the request body, supply a JSON representation of the [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md) object.</span></span> <span data-ttu-id="aec2f-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="aec2f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="aec2f-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="aec2f-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="aec2f-133">Para ver a lista de propriedades que podem ser atualizadas, consulte [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aec2f-133">For the list of properties that can be updated, see [emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="aec2f-134">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.emailAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="aec2f-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.emailAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="aec2f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec2f-135">Response</span></span>

<span data-ttu-id="aec2f-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aec2f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aec2f-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aec2f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aec2f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aec2f-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethodconfiguration"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email
Content-Type: application/json
Content-length: 147

{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "allowExternalIdToUseEmailOtp": "enabled",
}
```

### <a name="response"></a><span data-ttu-id="aec2f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="aec2f-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 NO CONTENT
```

