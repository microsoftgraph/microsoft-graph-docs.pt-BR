---
title: Atualizar identityApiConnector
description: Atualizar as propriedades de um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9037a6bfcd53af0ee009f232909a964a8b0e6a86
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873665"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="c4642-103">Atualizar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="c4642-103">Update identityApiConnector</span></span>

<span data-ttu-id="c4642-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4642-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4642-105">Atualizar as propriedades de um [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c4642-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4642-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4642-106">Permissions</span></span>

<span data-ttu-id="c4642-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4642-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4642-109">Permission type</span></span>                        | <span data-ttu-id="c4642-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4642-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c4642-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4642-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4642-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4642-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="c4642-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4642-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4642-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4642-114">Not supported.</span></span>  |
| <span data-ttu-id="c4642-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4642-115">Application</span></span>                            | <span data-ttu-id="c4642-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4642-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="c4642-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c4642-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c4642-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c4642-118">Global administrator</span></span>
* <span data-ttu-id="c4642-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="c4642-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c4642-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4642-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="c4642-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4642-121">Request headers</span></span>
|<span data-ttu-id="c4642-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c4642-122">Name</span></span>|<span data-ttu-id="c4642-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4642-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4642-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4642-124">Authorization</span></span>|<span data-ttu-id="c4642-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4642-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4642-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4642-127">Content-Type</span></span>|<span data-ttu-id="c4642-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4642-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4642-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4642-130">Request body</span></span>
<span data-ttu-id="c4642-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c4642-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="c4642-132">A tabela a seguir mostra as propriedades do [identityApiConnector](../resources/identityapiconnector.md) que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="c4642-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="c4642-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4642-133">Property</span></span>|<span data-ttu-id="c4642-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4642-134">Type</span></span>|<span data-ttu-id="c4642-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4642-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4642-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c4642-136">displayName</span></span>|<span data-ttu-id="c4642-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4642-137">String</span></span>| <span data-ttu-id="c4642-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="c4642-138">The name of the API connector.</span></span> |
|<span data-ttu-id="c4642-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="c4642-139">targetUrl</span></span>|<span data-ttu-id="c4642-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4642-140">String</span></span>| <span data-ttu-id="c4642-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="c4642-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="c4642-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4642-142">authenticationConfiguration</span></span>|[<span data-ttu-id="c4642-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="c4642-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="c4642-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="c4642-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="c4642-145">Somente [a autenticação](../resources/basicauthentication.md) Básica é suportada no momento.</span><span class="sxs-lookup"><span data-stu-id="c4642-145">Only [Basic authentication](../resources/basicauthentication.md) is supported at this time.</span></span> <span data-ttu-id="c4642-146">Todas as propriedades do apiAuthenticationConfigurationBase devem ser definidas ao mesmo tempo, como nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="c4642-146">All properties of the apiAuthenticationConfigurationBase must be set at the same time, like both username and password.</span></span>|

## <a name="response"></a><span data-ttu-id="c4642-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4642-147">Response</span></span>

<span data-ttu-id="c4642-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c4642-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c4642-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4642-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4642-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4642-150">Request</span></span>

<span data-ttu-id="c4642-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4642-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c4642-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4642-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4642-153">C#</span><span class="sxs-lookup"><span data-stu-id="c4642-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4642-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4642-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4642-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4642-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4642-156">Java</span><span class="sxs-lookup"><span data-stu-id="c4642-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4642-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4642-157">Response</span></span>

<span data-ttu-id="c4642-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4642-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
