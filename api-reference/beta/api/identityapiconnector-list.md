---
title: Listar identityApiConnectors
description: Obter uma lista dos objetos identityApiConnector e suas propriedades
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee208f75ce3629ea4217ae992e365578861d9aed
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874309"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="08221-103">Listar identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="08221-103">List identityApiConnectors</span></span>

<span data-ttu-id="08221-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08221-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08221-105">Leia as propriedades de um [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="08221-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08221-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="08221-106">Permissions</span></span>

<span data-ttu-id="08221-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08221-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08221-109">Permission type</span></span>                        | <span data-ttu-id="08221-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08221-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="08221-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08221-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08221-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08221-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="08221-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08221-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08221-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08221-114">Not supported.</span></span>  |
| <span data-ttu-id="08221-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08221-115">Application</span></span>                            | <span data-ttu-id="08221-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08221-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="08221-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="08221-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="08221-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="08221-118">Global administrator</span></span>
* <span data-ttu-id="08221-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="08221-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="08221-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08221-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08221-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08221-121">Optional query parameters</span></span>
<span data-ttu-id="08221-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08221-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="08221-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="08221-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="08221-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08221-124">Request headers</span></span>
|<span data-ttu-id="08221-125">Nome</span><span class="sxs-lookup"><span data-stu-id="08221-125">Name</span></span>|<span data-ttu-id="08221-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="08221-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="08221-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="08221-127">Authorization</span></span>|<span data-ttu-id="08221-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08221-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08221-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08221-130">Request body</span></span>
<span data-ttu-id="08221-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08221-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08221-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="08221-132">Response</span></span>

<span data-ttu-id="08221-133">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08221-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08221-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08221-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="08221-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08221-135">Request</span></span>

<span data-ttu-id="08221-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08221-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08221-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="08221-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="08221-138">C#</span><span class="sxs-lookup"><span data-stu-id="08221-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08221-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08221-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08221-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08221-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08221-141">Java</span><span class="sxs-lookup"><span data-stu-id="08221-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08221-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="08221-142">Response</span></span>

<span data-ttu-id="08221-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08221-143">The following is an example of the response.</span></span>

<span data-ttu-id="08221-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="08221-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "<guid>",
          "displayName": "Test API",
          "targetUrl": "https://someapi.com/api/endpoint",
          "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
          }
      }
  ]
}
```
