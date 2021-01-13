---
title: Criar identityApiConnector
description: Criar um novo objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fac7a1179bfbe7634df1194543112f5a2c5b36d6
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844524"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="08a6b-103">Criar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="08a6b-103">Create identityApiConnector</span></span>

<span data-ttu-id="08a6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08a6b-105">Criar um novo [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="08a6b-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08a6b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="08a6b-106">Permissions</span></span>

<span data-ttu-id="08a6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08a6b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08a6b-109">Permission type</span></span>                        | <span data-ttu-id="08a6b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08a6b-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="08a6b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08a6b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08a6b-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a6b-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="08a6b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08a6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08a6b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08a6b-114">Not supported.</span></span>  |
| <span data-ttu-id="08a6b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08a6b-115">Application</span></span>                            | <span data-ttu-id="08a6b-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08a6b-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="08a6b-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="08a6b-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="08a6b-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="08a6b-118">Global administrator</span></span>
* <span data-ttu-id="08a6b-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="08a6b-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="08a6b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08a6b-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="08a6b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08a6b-121">Request headers</span></span>

| <span data-ttu-id="08a6b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="08a6b-122">Name</span></span>          | <span data-ttu-id="08a6b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a6b-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="08a6b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="08a6b-124">Authorization</span></span> | <span data-ttu-id="08a6b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a6b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="08a6b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08a6b-127">Content-Type</span></span>  | <span data-ttu-id="08a6b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08a6b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08a6b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08a6b-130">Request body</span></span>

<span data-ttu-id="08a6b-131">No corpo da solicitação, fornece uma representação JSON do [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="08a6b-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="08a6b-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityApiConnector](../resources/identityapiconnector.md).</span><span class="sxs-lookup"><span data-stu-id="08a6b-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="08a6b-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08a6b-133">Property</span></span>|<span data-ttu-id="08a6b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="08a6b-134">Type</span></span>|<span data-ttu-id="08a6b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="08a6b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08a6b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="08a6b-136">displayName</span></span>|<span data-ttu-id="08a6b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08a6b-137">String</span></span>| <span data-ttu-id="08a6b-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="08a6b-138">The name of the API connector.</span></span> |
|<span data-ttu-id="08a6b-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="08a6b-139">targetUrl</span></span>|<span data-ttu-id="08a6b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08a6b-140">String</span></span>| <span data-ttu-id="08a6b-141">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="08a6b-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="08a6b-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="08a6b-142">authenticationConfiguration</span></span>|[<span data-ttu-id="08a6b-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="08a6b-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="08a6b-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="08a6b-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="08a6b-145">Somente [a autenticação Básica](../resources/basicauthentication.md) é suportada.</span><span class="sxs-lookup"><span data-stu-id="08a6b-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="08a6b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a6b-146">Response</span></span>

<span data-ttu-id="08a6b-147">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08a6b-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08a6b-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08a6b-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08a6b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08a6b-149">Request</span></span>

<span data-ttu-id="08a6b-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08a6b-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08a6b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="08a6b-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08a6b-152">C#</span><span class="sxs-lookup"><span data-stu-id="08a6b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08a6b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08a6b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08a6b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08a6b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08a6b-155">Java</span><span class="sxs-lookup"><span data-stu-id="08a6b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08a6b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="08a6b-156">Response</span></span>

<span data-ttu-id="08a6b-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08a6b-157">The following is an example of the response.</span></span>

<span data-ttu-id="08a6b-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="08a6b-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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
