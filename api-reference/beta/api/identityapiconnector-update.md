---
title: Atualizar identityApiConnector
description: Atualizar as propriedades de um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5fd0c263d81c0fa03c31743465453194618d99c2
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844331"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="54c09-103">Atualizar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="54c09-103">Update identityApiConnector</span></span>

<span data-ttu-id="54c09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54c09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54c09-105">Atualizar as propriedades de um [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="54c09-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54c09-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="54c09-106">Permissions</span></span>

<span data-ttu-id="54c09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54c09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54c09-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54c09-109">Permission type</span></span>                        | <span data-ttu-id="54c09-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54c09-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="54c09-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54c09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54c09-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c09-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="54c09-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54c09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54c09-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54c09-114">Not supported.</span></span>  |
| <span data-ttu-id="54c09-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54c09-115">Application</span></span>                            | <span data-ttu-id="54c09-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c09-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="54c09-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="54c09-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="54c09-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="54c09-118">Global administrator</span></span>
* <span data-ttu-id="54c09-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="54c09-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="54c09-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54c09-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="54c09-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54c09-121">Request headers</span></span>
|<span data-ttu-id="54c09-122">Nome</span><span class="sxs-lookup"><span data-stu-id="54c09-122">Name</span></span>|<span data-ttu-id="54c09-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c09-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="54c09-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="54c09-124">Authorization</span></span>|<span data-ttu-id="54c09-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54c09-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="54c09-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54c09-127">Content-Type</span></span>|<span data-ttu-id="54c09-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54c09-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="54c09-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54c09-130">Request body</span></span>
<span data-ttu-id="54c09-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="54c09-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="54c09-132">A tabela a seguir mostra as propriedades do [identityApiConnector](../resources/identityapiconnector.md) que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="54c09-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="54c09-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54c09-133">Property</span></span>|<span data-ttu-id="54c09-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="54c09-134">Type</span></span>|<span data-ttu-id="54c09-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c09-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54c09-136">displayName</span><span class="sxs-lookup"><span data-stu-id="54c09-136">displayName</span></span>|<span data-ttu-id="54c09-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54c09-137">String</span></span>| <span data-ttu-id="54c09-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="54c09-138">The name of the API connector.</span></span> |
|<span data-ttu-id="54c09-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="54c09-139">targetUrl</span></span>|<span data-ttu-id="54c09-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54c09-140">String</span></span>| <span data-ttu-id="54c09-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="54c09-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="54c09-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="54c09-142">authenticationConfiguration</span></span>|[<span data-ttu-id="54c09-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="54c09-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="54c09-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="54c09-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="54c09-145">Somente [a autenticação](../resources/basicauthentication.md) Básica é suportada no momento.</span><span class="sxs-lookup"><span data-stu-id="54c09-145">Only [Basic authentication](../resources/basicauthentication.md) is supported at this time.</span></span> <span data-ttu-id="54c09-146">Todas as propriedades do apiAuthenticationConfigurationBase devem ser definidas ao mesmo tempo, como nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="54c09-146">All properties of the apiAuthenticationConfigurationBase must be set at the same time, like both username and password.</span></span>|

## <a name="response"></a><span data-ttu-id="54c09-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c09-147">Response</span></span>

<span data-ttu-id="54c09-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="54c09-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="54c09-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54c09-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54c09-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54c09-150">Request</span></span>

<span data-ttu-id="54c09-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54c09-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54c09-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="54c09-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="54c09-153">C#</span><span class="sxs-lookup"><span data-stu-id="54c09-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54c09-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54c09-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54c09-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54c09-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54c09-156">Java</span><span class="sxs-lookup"><span data-stu-id="54c09-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54c09-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c09-157">Response</span></span>

<span data-ttu-id="54c09-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54c09-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
