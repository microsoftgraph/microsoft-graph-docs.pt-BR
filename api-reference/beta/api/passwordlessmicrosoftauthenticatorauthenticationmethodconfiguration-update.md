---
title: Atualizar passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Atualiza as propriedades de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8536e70f264775a073830aeac77d3fc27810e5f0
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418210"
---
# <a name="update-passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration"></a><span data-ttu-id="1fc0e-103">Atualizar passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fc0e-103">Update passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="1fc0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fc0e-105">Atualize as propriedades do objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) , que representa a política de método de autenticação de entrada de telefone sem senha do Microsoft Authenticator para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-105">Update the properties of the [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object, which represents the Microsoft Authenticator Passwordless Phone Sign-in authentication method policy for the Azure AD tenant.</span></span>

> [!NOTE]
> <span data-ttu-id="1fc0e-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="1fc0e-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fc0e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fc0e-108">Permissions</span></span>
<span data-ttu-id="1fc0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fc0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc0e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fc0e-111">Permission type</span></span>|<span data-ttu-id="1fc0e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1fc0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fc0e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fc0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fc0e-114">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1fc0e-114">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="1fc0e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fc0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fc0e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-116">Not supported.</span></span>|
|<span data-ttu-id="1fc0e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fc0e-117">Application</span></span>|<span data-ttu-id="1fc0e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-118">Not supported.</span></span>|

<span data-ttu-id="1fc0e-119">Para cenários delegados, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1fc0e-119">For delegated scenarios, the administrator needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1fc0e-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1fc0e-120">Global admin</span></span>
* <span data-ttu-id="1fc0e-121">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1fc0e-121">Global reader</span></span>
* <span data-ttu-id="1fc0e-122">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1fc0e-122">Privileged authentication admin</span></span>
* <span data-ttu-id="1fc0e-123">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="1fc0e-123">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1fc0e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fc0e-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator
```

## <a name="request-headers"></a><span data-ttu-id="1fc0e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc0e-125">Request headers</span></span>
|<span data-ttu-id="1fc0e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="1fc0e-126">Name</span></span>|<span data-ttu-id="1fc0e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fc0e-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1fc0e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fc0e-128">Authorization</span></span>|<span data-ttu-id="1fc0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1fc0e-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fc0e-131">Content-Type</span></span>|<span data-ttu-id="1fc0e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc0e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc0e-134">Request body</span></span>
<span data-ttu-id="1fc0e-135">No corpo da solicitação, forneça uma representação JSON de um objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-135">In the request body, supply a JSON representation of a [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="1fc0e-136">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-136">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1fc0e-137">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-137">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="1fc0e-138">Para obter a lista de propriedades, consulte [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1fc0e-138">For the list of properties, see [passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="1fc0e-139">**Observação:** A `@odata.type` propriedade com um valor de `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` deve ser incluída no corpo.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-139">**Note:** The `@odata.type` property with a value of `#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="1fc0e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fc0e-140">Response</span></span>

<span data-ttu-id="1fc0e-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fc0e-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fc0e-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fc0e-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1fc0e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fc0e-144">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="1fc0e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fc0e-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

