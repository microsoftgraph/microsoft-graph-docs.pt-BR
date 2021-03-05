---
title: Atualizar smsAuthenticationMethodConfiguration
description: Atualize as propriedades de um objeto smsAuthenticationMethodConfiguration.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbdcddf77f2e85517b6c8d1685b4129b1e8d83f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475587"
---
# <a name="update-smsauthenticationmethodconfiguration"></a><span data-ttu-id="dc417-103">Atualizar smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc417-103">Update smsAuthenticationMethodConfiguration</span></span>
<span data-ttu-id="dc417-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc417-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc417-105">Atualize as propriedades de um [objeto smsAuthenticationMethodConfiguration,](../resources/smsauthenticationmethodconfiguration.md) que representa a política de método de autenticação de Mensagem de Texto para o locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc417-105">Update the properties of a [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object, which represents the Text Message authentication method policy for the Azure AD tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc417-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc417-106">Permissions</span></span>
<span data-ttu-id="dc417-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc417-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc417-109">Permission type</span></span>|<span data-ttu-id="dc417-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc417-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc417-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc417-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc417-112">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dc417-112">Policy.ReadWrite.AuthenticationMethod</span></span>|
|<span data-ttu-id="dc417-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc417-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc417-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc417-114">Not supported.</span></span>|
|<span data-ttu-id="dc417-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc417-115">Application</span></span>|<span data-ttu-id="dc417-116">Policy.ReadWrite.AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dc417-116">Policy.ReadWrite.AuthenticationMethod</span></span>|

<span data-ttu-id="dc417-117">Para cenários delegados, o administrador precisa da função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="dc417-117">For delegated scenarios, the administrator needs the Global admin role.</span></span> <span data-ttu-id="dc417-118">Para obter mais informações, consulte [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="dc417-118">For more information, see [role](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="dc417-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc417-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
```

## <a name="request-headers"></a><span data-ttu-id="dc417-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc417-120">Request headers</span></span>
|<span data-ttu-id="dc417-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dc417-121">Name</span></span>|<span data-ttu-id="dc417-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc417-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc417-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc417-123">Authorization</span></span>|<span data-ttu-id="dc417-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc417-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dc417-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc417-126">Content-Type</span></span>|<span data-ttu-id="dc417-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc417-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc417-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc417-129">Request body</span></span>
<span data-ttu-id="dc417-130">No corpo da solicitação, fornece uma representação JSON do [objeto smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) com os valores dos campos que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="dc417-130">In the request body, supply a JSON representation of the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object with the values of fields that should be updated.</span></span> <span data-ttu-id="dc417-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="dc417-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="dc417-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="dc417-132">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="dc417-133">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [objeto smsAuthenticationMethodConfiguration.](../resources/smsauthenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc417-133">The following table shows the properties that are required when you update the [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object.</span></span>

|<span data-ttu-id="dc417-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc417-134">Property</span></span>|<span data-ttu-id="dc417-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc417-135">Type</span></span>|<span data-ttu-id="dc417-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc417-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc417-137">id</span><span class="sxs-lookup"><span data-stu-id="dc417-137">id</span></span>|<span data-ttu-id="dc417-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc417-138">String</span></span>|<span data-ttu-id="dc417-139">O identificador de política do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="dc417-139">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="dc417-140">estado</span><span class="sxs-lookup"><span data-stu-id="dc417-140">state</span></span>|<span data-ttu-id="dc417-141">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="dc417-141">authenticationMethodState</span></span>|<span data-ttu-id="dc417-142">Os valores possíveis são: `enabled` e `disabled`.</span><span class="sxs-lookup"><span data-stu-id="dc417-142">Possible values are: `enabled`, `disabled`.</span></span>|

><span data-ttu-id="dc417-143">**Observação:** A `@odata.type` propriedade com um valor de deve ser incluída no `#microsoft.graph.smsAuthenticationMethodConfiguration` corpo.</span><span class="sxs-lookup"><span data-stu-id="dc417-143">**Note:** The `@odata.type` property with a value of `#microsoft.graph.smsAuthenticationMethodConfiguration` must be included in the body.</span></span>

## <a name="response"></a><span data-ttu-id="dc417-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc417-144">Response</span></span>

<span data-ttu-id="dc417-145">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc417-145">If successful, this method returns a `200 OK` response code and an updated [smsAuthenticationMethodConfiguration](../resources/smsauthenticationmethodconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc417-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc417-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc417-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc417-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dc417-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc417-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethodconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms
Content-Type: application/json
Content-length: 100

{
    "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
    "id": "Sms",
    "state": "enabled"
}
```
# <a name="c"></a>[<span data-ttu-id="dc417-149">C#</span><span class="sxs-lookup"><span data-stu-id="dc417-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-smsauthenticationmethodconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc417-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc417-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-smsauthenticationmethodconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc417-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc417-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-smsauthenticationmethodconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc417-152">Java</span><span class="sxs-lookup"><span data-stu-id="dc417-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-smsauthenticationmethodconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dc417-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc417-153">Response</span></span>
<span data-ttu-id="dc417-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc417-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.smsAuthenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodConfiguration",
  "id": "713980c7-80c7-7139-c780-3971c7803971",
  "state": "String"
}
```

