---
title: Atualizar fido2AuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto fido2AuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c5c66ebea0bb4f544fae01525dc113e8bf11ed23
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471058"
---
# <a name="update-fido2authenticationmethodconfiguration"></a><span data-ttu-id="4127c-103">Atualizar fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="4127c-103">Update fido2AuthenticationMethodConfiguration</span></span>
<span data-ttu-id="4127c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4127c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4127c-105">Atualize as propriedades de um objeto [fido2AuthenticationMethodConfiguration,](../resources/fido2authenticationmethodconfiguration.md) que representa a política de método de autenticação de Chaves de Segurança FIDO2 para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4127c-105">Update the properties of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object, which represents the FIDO2 Security Keys authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4127c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4127c-106">Permissions</span></span>
<span data-ttu-id="4127c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4127c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4127c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4127c-109">Permission type</span></span>|<span data-ttu-id="4127c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4127c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4127c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4127c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4127c-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4127c-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="4127c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4127c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4127c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4127c-114">Not supported.</span></span>|
|<span data-ttu-id="4127c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4127c-115">Application</span></span>|<span data-ttu-id="4127c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4127c-116">Not supported.</span></span>|

<span data-ttu-id="4127c-117">Para cenários delegados, o administrador precisa da seguinte [função:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="4127c-117">For delegated scenarios, the administrator needs the following [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4127c-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4127c-118">Global admin</span></span>


## <a name="http-request"></a><span data-ttu-id="4127c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4127c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
```

## <a name="request-headers"></a><span data-ttu-id="4127c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4127c-120">Request headers</span></span>
|<span data-ttu-id="4127c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4127c-121">Name</span></span>|<span data-ttu-id="4127c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4127c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4127c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4127c-123">Authorization</span></span>|<span data-ttu-id="4127c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4127c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4127c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4127c-126">Content-Type</span></span>|<span data-ttu-id="4127c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4127c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4127c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4127c-129">Request body</span></span>
<span data-ttu-id="4127c-130">No corpo da solicitação, fornece uma representação JSON de um [objeto fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) com os valores de campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4127c-130">In the request body, supply a JSON representation of a [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="4127c-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4127c-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4127c-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4127c-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="4127c-133">Para ver a lista de propriedades que podem ser atualizadas, consulte [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4127c-133">For the list of properties that can be updated, see [fido2AuthenticationMethodConfiguration](../resources/fido2authenticationmethodconfiguration.md).</span></span>

><span data-ttu-id="4127c-134">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.fido2AuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="4127c-134">**Note:** The `@odata.type` property with a value of `#microsoft.graph.fido2AuthenticationMethodConfiguration` must be included in the body.</span></span>


## <a name="response"></a><span data-ttu-id="4127c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4127c-135">Response</span></span>

<span data-ttu-id="4127c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4127c-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4127c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4127c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4127c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4127c-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4127c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4127c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_fido2authenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    "state": "enabled",
    "isAttestationEnforced": "true"
}
```
# <a name="c"></a>[<span data-ttu-id="4127c-141">C#</span><span class="sxs-lookup"><span data-stu-id="4127c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-fido2authenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4127c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4127c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-fido2authenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4127c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4127c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-fido2authenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4127c-144">Java</span><span class="sxs-lookup"><span data-stu-id="4127c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-fido2authenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4127c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4127c-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

