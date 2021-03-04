---
title: Atualizar passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Atualize as propriedades de um objetoMicrosoftAuthenticatorAuthenticationMethodConfiguration sem senha.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9093e049eab262df56c914bdb735e9d9600b799d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447665"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-deprecated"></a><span data-ttu-id="fea13-103">Atualizar passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (preterido)</span><span class="sxs-lookup"><span data-stu-id="fea13-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (deprecated)</span></span>
<span data-ttu-id="fea13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fea13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea13-105">Atualize as propriedades do objeto [PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration,](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) que representa a política de autenticação de autenticação de telefone sem senha do Microsoft Authenticator Passwordless Phone Sign-in para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fea13-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!CAUTION]
> <span data-ttu-id="fea13-106">A API de política de autenticação do método de autenticação de telefone sem senha do Microsoft Authenticator é preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="fea13-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="fea13-107">Use a nova política de método de autenticação do [Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fea13-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fea13-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fea13-108">Permissions</span></span>
<span data-ttu-id="fea13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fea13-111">Permission type</span></span>|<span data-ttu-id="fea13-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fea13-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea13-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fea13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fea13-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fea13-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="fea13-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fea13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea13-116">Not supported.</span></span>|
|<span data-ttu-id="fea13-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fea13-117">Application</span></span>|<span data-ttu-id="fea13-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fea13-118">Not supported.</span></span>|

<span data-ttu-id="fea13-119">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="fea13-119">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="fea13-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fea13-120">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="fea13-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fea13-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="fea13-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fea13-122">Request headers</span></span>
|<span data-ttu-id="fea13-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fea13-123">Name</span></span>|<span data-ttu-id="fea13-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fea13-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fea13-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fea13-125">Authorization</span></span>|<span data-ttu-id="fea13-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea13-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fea13-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fea13-128">Content-Type</span></span>|<span data-ttu-id="fea13-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fea13-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea13-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fea13-131">Request body</span></span>
<span data-ttu-id="fea13-132">No corpo da solicitação, fornece uma representação JSON de um [objetoMicrosoftAuthenticatorAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="fea13-132">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="fea13-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="fea13-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fea13-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fea13-134">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="fea13-135">Para ver a lista de propriedades, consulte [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fea13-135">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="fea13-136">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="fea13-136">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="fea13-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea13-137">Response</span></span>

<span data-ttu-id="fea13-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fea13-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fea13-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fea13-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fea13-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fea13-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    "state": "enabled"
}
```


### <a name="response"></a><span data-ttu-id="fea13-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fea13-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

