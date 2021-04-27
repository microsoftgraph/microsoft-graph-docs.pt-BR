---
title: Atualizar temporaryAccessPassAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6cd30c6016739fcb40c3d6541b1fd1b03f72bee6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049636"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="6bb45-103">Atualizar temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bb45-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="6bb45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bb45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bb45-105">Atualize as propriedades de [um objeto temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) que representa a política de método de autenticação Passagem de Acesso Temporário para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6bb45-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bb45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bb45-106">Permissions</span></span>
<span data-ttu-id="6bb45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bb45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bb45-109">Permission type</span></span>|<span data-ttu-id="6bb45-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bb45-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bb45-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bb45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bb45-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6bb45-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="6bb45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bb45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bb45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bb45-114">Not supported.</span></span>|
|<span data-ttu-id="6bb45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bb45-115">Application</span></span>|<span data-ttu-id="6bb45-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6bb45-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="6bb45-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="6bb45-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="6bb45-118">Para obter mais informações, consulte[funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="6bb45-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="6bb45-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb45-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="6bb45-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb45-120">Request headers</span></span>
|<span data-ttu-id="6bb45-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6bb45-121">Name</span></span>|<span data-ttu-id="6bb45-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bb45-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6bb45-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bb45-123">Authorization</span></span>|<span data-ttu-id="6bb45-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bb45-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6bb45-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6bb45-126">Content-Type</span></span>|<span data-ttu-id="6bb45-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bb45-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bb45-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb45-129">Request body</span></span>
<span data-ttu-id="6bb45-130">No corpo da solicitação, fornece uma representação JSON do [objeto temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6bb45-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="6bb45-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6bb45-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6bb45-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6bb45-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="6bb45-133">Todas as propriedades do objeto podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="6bb45-133">All properties of the object can be updated.</span></span> <span data-ttu-id="6bb45-134">Para uma lista de propriedades, consulte [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bb45-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="6bb45-135">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="6bb45-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="6bb45-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb45-136">Response</span></span>

<span data-ttu-id="6bb45-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bb45-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bb45-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6bb45-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6bb45-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bb45-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6bb45-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb45-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_temporaryaccesspassauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
Content-Type: application/json

{
  "@odata.type":"#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "state":"enabled",
  "defaultLifetimeInMinutes":60,
  "defaultLength":8,
  "minimumLifetimeInMinutes":60,
  "maximumLifetimeInMinutes":1440,"
  isUsableOnce":false,
  "includeTargets": [
        {
            "targetType": "group",
            "id": "all_users",
            "isRegistrationRequired": false,
            "useForSignIn": true
        }
    ]
}


```
# <a name="javascript"></a>[<span data-ttu-id="6bb45-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bb45-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-temporaryaccesspassauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bb45-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bb45-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-temporaryaccesspassauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bb45-144">Java</span><span class="sxs-lookup"><span data-stu-id="6bb45-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-temporaryaccesspassauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bb45-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bb45-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
