---
title: Atualizar temporaryAccessPassAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto temporaryAccessPassAuthenticationMethodConfiguration.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1d8d888f71fd59b8b2b00cd45c2c88151e940aea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761762"
---
# <a name="update-temporaryaccesspassauthenticationmethodconfiguration"></a><span data-ttu-id="4963f-103">Atualizar temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4963f-103">Update temporaryAccessPassAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4963f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4963f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4963f-105">Atualize as propriedades de [um objeto temporaryAccessPassAuthenticationMethodConfiguration,](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) que representa a política de método de autenticação Passagem de Acesso Temporário para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4963f-105">Update the properties of a [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object,  which represents the Temporary Access Pass authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4963f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4963f-106">Permissions</span></span>
<span data-ttu-id="4963f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4963f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4963f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4963f-109">Permission type</span></span>|<span data-ttu-id="4963f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4963f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4963f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4963f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4963f-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4963f-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4963f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4963f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4963f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4963f-114">Not supported.</span></span>|
|<span data-ttu-id="4963f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4963f-115">Application</span></span>|<span data-ttu-id="4963f-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4963f-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

 <span data-ttu-id="4963f-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="4963f-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="4963f-118">Para obter mais informações, consulte[funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="4963f-118">For more information, see[roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>


## <a name="http-request"></a><span data-ttu-id="4963f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4963f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass
```

## <a name="request-headers"></a><span data-ttu-id="4963f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4963f-120">Request headers</span></span>
|<span data-ttu-id="4963f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4963f-121">Name</span></span>|<span data-ttu-id="4963f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4963f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4963f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4963f-123">Authorization</span></span>|<span data-ttu-id="4963f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4963f-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4963f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4963f-126">Content-Type</span></span>|<span data-ttu-id="4963f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4963f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4963f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4963f-129">Request body</span></span>
<span data-ttu-id="4963f-130">No corpo da solicitação, fornece uma representação JSON do [objeto temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4963f-130">In the request body, supply a JSON representation of the [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="4963f-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4963f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4963f-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4963f-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4963f-133">Todas as propriedades do objeto podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="4963f-133">All properties of the object can be updated.</span></span> <span data-ttu-id="4963f-134">Para uma lista de propriedades, consulte [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4963f-134">For a list of properties, see [temporaryAccessPassAuthenticationMethodConfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="4963f-135">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="4963f-135">**Note:** The `@odata.type` property with a value of `#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="4963f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4963f-136">Response</span></span>

<span data-ttu-id="4963f-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4963f-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4963f-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4963f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4963f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4963f-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4963f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4963f-141">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="4963f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4963f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-temporaryaccesspassauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4963f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4963f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-temporaryaccesspassauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4963f-144">Java</span><span class="sxs-lookup"><span data-stu-id="4963f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-temporaryaccesspassauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4963f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4963f-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
