---
title: Criar identityApiConnector
description: Crie um novo objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e2ff03ae081a1d406a56c5a826664bb402983a4f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435607"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="750b4-103">Criar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="750b4-103">Create identityApiConnector</span></span>

<span data-ttu-id="750b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="750b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="750b4-105">Crie um novo [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="750b4-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="750b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="750b4-106">Permissions</span></span>

<span data-ttu-id="750b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="750b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="750b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="750b4-109">Permission type</span></span>                        | <span data-ttu-id="750b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="750b4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="750b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="750b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="750b4-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="750b4-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="750b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="750b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="750b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="750b4-114">Not supported.</span></span>  |
| <span data-ttu-id="750b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="750b4-115">Application</span></span>                            | <span data-ttu-id="750b4-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="750b4-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="750b4-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="750b4-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="750b4-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="750b4-118">Global administrator</span></span>
* <span data-ttu-id="750b4-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="750b4-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="750b4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="750b4-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="750b4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="750b4-121">Request headers</span></span>

| <span data-ttu-id="750b4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="750b4-122">Name</span></span>          | <span data-ttu-id="750b4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="750b4-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="750b4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="750b4-124">Authorization</span></span> | <span data-ttu-id="750b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="750b4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="750b4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="750b4-127">Content-Type</span></span>  | <span data-ttu-id="750b4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="750b4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="750b4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="750b4-130">Request body</span></span>

<span data-ttu-id="750b4-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="750b4-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="750b4-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityApiConnector](../resources/identityapiconnector.md).</span><span class="sxs-lookup"><span data-stu-id="750b4-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="750b4-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="750b4-133">Property</span></span>|<span data-ttu-id="750b4-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="750b4-134">Type</span></span>|<span data-ttu-id="750b4-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="750b4-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="750b4-136">displayName</span></span>|<span data-ttu-id="750b4-137">String</span><span class="sxs-lookup"><span data-stu-id="750b4-137">String</span></span>| <span data-ttu-id="750b4-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="750b4-138">The name of the API connector.</span></span> |
|<span data-ttu-id="750b4-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="750b4-139">targetUrl</span></span>|<span data-ttu-id="750b4-140">String</span><span class="sxs-lookup"><span data-stu-id="750b4-140">String</span></span>| <span data-ttu-id="750b4-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="750b4-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="750b4-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="750b4-142">authenticationConfiguration</span></span>|[<span data-ttu-id="750b4-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="750b4-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="750b4-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="750b4-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="750b4-145">Somente [a autenticação básica](../resources/basicauthentication.md) é suportada.</span><span class="sxs-lookup"><span data-stu-id="750b4-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="750b4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="750b4-146">Response</span></span>

<span data-ttu-id="750b4-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="750b4-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="750b4-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="750b4-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="750b4-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="750b4-149">Request</span></span>

<span data-ttu-id="750b4-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="750b4-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="750b4-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="750b4-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="750b4-152">C#</span><span class="sxs-lookup"><span data-stu-id="750b4-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="750b4-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="750b4-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="750b4-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="750b4-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="750b4-155">Java</span><span class="sxs-lookup"><span data-stu-id="750b4-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="750b4-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="750b4-156">Response</span></span>

<span data-ttu-id="750b4-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="750b4-157">The following is an example of the response.</span></span>

<span data-ttu-id="750b4-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="750b4-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
