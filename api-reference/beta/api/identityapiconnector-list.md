---
title: Listar identityApiConnectors
description: Obter uma lista dos objetos identityApiConnector e suas propriedades
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6aa2d3a4a5c45dc7b9e0b168eac7402404fcb982
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507844"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="e8a67-103">Listar identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="e8a67-103">List identityApiConnectors</span></span>

<span data-ttu-id="e8a67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8a67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a67-105">Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="e8a67-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a67-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8a67-106">Permissions</span></span>

<span data-ttu-id="e8a67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8a67-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8a67-109">Permission type</span></span>                        | <span data-ttu-id="e8a67-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8a67-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e8a67-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8a67-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8a67-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a67-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="e8a67-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8a67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a67-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8a67-114">Not supported.</span></span>  |
| <span data-ttu-id="e8a67-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8a67-115">Application</span></span>                            | <span data-ttu-id="e8a67-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a67-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="e8a67-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e8a67-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e8a67-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e8a67-118">Global administrator</span></span>
* <span data-ttu-id="e8a67-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="e8a67-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e8a67-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a67-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8a67-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8a67-121">Optional query parameters</span></span>
<span data-ttu-id="e8a67-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a67-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8a67-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8a67-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8a67-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a67-124">Request headers</span></span>
|<span data-ttu-id="e8a67-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e8a67-125">Name</span></span>|<span data-ttu-id="e8a67-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8a67-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e8a67-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8a67-127">Authorization</span></span>|<span data-ttu-id="e8a67-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8a67-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8a67-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a67-130">Request body</span></span>
<span data-ttu-id="e8a67-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8a67-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a67-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a67-132">Response</span></span>

<span data-ttu-id="e8a67-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a67-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8a67-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8a67-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8a67-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a67-135">Request</span></span>

<span data-ttu-id="e8a67-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8a67-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8a67-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a67-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="e8a67-138">C#</span><span class="sxs-lookup"><span data-stu-id="e8a67-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8a67-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8a67-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8a67-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8a67-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8a67-141">Java</span><span class="sxs-lookup"><span data-stu-id="e8a67-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8a67-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a67-142">Response</span></span>

<span data-ttu-id="e8a67-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a67-143">The following is an example of the response.</span></span>

<span data-ttu-id="e8a67-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8a67-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        },
        {
            "id": "<guid>",
            "displayName": "My API connector",
            "targetUrl": "https://someotherapi.com/api/endpoint",
            "authenticationConfiguration": {
                "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
                "certificateList": [
                    {
                        "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                        "notAfter": 1666350522,
                        "notBefore": 1508670522,
                        "isActive": true
                    },
                    {
                        "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                        "notAfter": 1766350522,
                        "notBefore": 1608670522,
                        "isActive": false
                    }
                ]
            }
        }
  ]
}
```
