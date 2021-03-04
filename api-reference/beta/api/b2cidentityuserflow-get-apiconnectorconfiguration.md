---
title: Obter userFlowApiConnectorConfiguration
description: Obter a propriedade userFlowApiConnectorConfiguration de um b2cIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d582b55a37845a855e79ff90e8eb510f50c4e03e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438320"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="53f30-103">Obter userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="53f30-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="53f30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53f30-105">Obter a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2cIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) para detalhar os conectores de API habilitados para o fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="53f30-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2cIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="53f30-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="53f30-106">Permissions</span></span>

<span data-ttu-id="53f30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53f30-109">Permission type</span></span>      | <span data-ttu-id="53f30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53f30-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53f30-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53f30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53f30-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f30-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="53f30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53f30-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="53f30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53f30-114">Not supported.</span></span>|
|<span data-ttu-id="53f30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53f30-115">Application</span></span>|<span data-ttu-id="53f30-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53f30-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="53f30-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="53f30-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="53f30-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="53f30-118">Global administrator</span></span>
* <span data-ttu-id="53f30-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="53f30-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="53f30-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53f30-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2cUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53f30-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="53f30-121">Optional query parameters</span></span>

<span data-ttu-id="53f30-122">Este método dá suporte ao `$expand` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="53f30-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="53f30-123">Por exemplo, para recuperar o conector de API para as `postFederationSignup` etapas `postAttributeCollection` e, adicione `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="53f30-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="53f30-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="53f30-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53f30-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53f30-125">Request headers</span></span>

|<span data-ttu-id="53f30-126">Nome</span><span class="sxs-lookup"><span data-stu-id="53f30-126">Name</span></span>|<span data-ttu-id="53f30-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="53f30-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53f30-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="53f30-128">Authorization</span></span>|<span data-ttu-id="53f30-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53f30-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f30-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53f30-131">Request body</span></span>

<span data-ttu-id="53f30-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53f30-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53f30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="53f30-133">Response</span></span>

<span data-ttu-id="53f30-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53f30-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="53f30-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="53f30-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53f30-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53f30-136">Request</span></span>

<span data-ttu-id="53f30-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="53f30-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53f30-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="53f30-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```
# <a name="c"></a>[<span data-ttu-id="53f30-139">C#</span><span class="sxs-lookup"><span data-stu-id="53f30-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-apiconnectorconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53f30-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53f30-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-apiconnectorconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53f30-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53f30-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-apiconnectorconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53f30-142">Java</span><span class="sxs-lookup"><span data-stu-id="53f30-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflows-apiconnectorconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53f30-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="53f30-143">Response</span></span>

<span data-ttu-id="53f30-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="53f30-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
    "postFederationSignup": {
        "id": "<guid1>",
        "displayName": "Test API Connector 1",
        "targetUrl": "https://someapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
        }
    },
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
    "postAttributeCollection": {
        "id": "<guid2>",
        "displayName": "Test API Connector 2",
        "targetUrl": "https://someotherapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME2>",
            "password": "******"
        }
    }
}
```
