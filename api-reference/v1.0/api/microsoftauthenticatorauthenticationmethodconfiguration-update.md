---
title: Atualizar microsoftAuthenticatorAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto microsoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f171b15480d04ef88ed6c3f35ea3ff4f6f03c6b1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948956"
---
# <a name="update-microsoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="1d62d-103">Atualizar microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d62d-103">Update microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1d62d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d62d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d62d-105">Atualize as propriedades de um [objeto microsoftAuthenticatorAuthenticationMethodConfiguration,](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) que representa a política de método de autenticação do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d62d-105">Update the properties of a [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator authentication method policy for the Azure AD tenant.</span></span>


## <a name="permissions"></a><span data-ttu-id="1d62d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d62d-106">Permissions</span></span>
<span data-ttu-id="1d62d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d62d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d62d-109">Permission type</span></span>|<span data-ttu-id="1d62d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d62d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d62d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d62d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d62d-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1d62d-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1d62d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d62d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d62d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d62d-114">Not supported.</span></span>|
|<span data-ttu-id="1d62d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d62d-115">Application</span></span>|<span data-ttu-id="1d62d-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1d62d-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="1d62d-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="1d62d-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="1d62d-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="1d62d-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="1d62d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d62d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="1d62d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d62d-120">Request headers</span></span>
|<span data-ttu-id="1d62d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1d62d-121">Name</span></span>|<span data-ttu-id="1d62d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d62d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d62d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d62d-123">Authorization</span></span>|<span data-ttu-id="1d62d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d62d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1d62d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d62d-126">Content-Type</span></span>|<span data-ttu-id="1d62d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d62d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d62d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d62d-129">Request body</span></span>
<span data-ttu-id="1d62d-130">No corpo da solicitação, fornece uma representação JSON do [objeto microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) com os valores de campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1d62d-130">In the request body, supply a JSON representation of the [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="1d62d-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1d62d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1d62d-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1d62d-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="1d62d-133">Para ver a lista de propriedades, consulte [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d62d-133">For the list of properties, see [microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="1d62d-134">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="1d62d-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="1d62d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d62d-135">Response</span></span>

<span data-ttu-id="1d62d-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d62d-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d62d-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d62d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d62d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d62d-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_microsoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "state": "String"
}
```


### <a name="response"></a><span data-ttu-id="1d62d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d62d-140">Response</span></span>
<span data-ttu-id="1d62d-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d62d-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "129ae788-e788-129a-88e7-9a1288e79a12",
  "state": "String"
}
```

