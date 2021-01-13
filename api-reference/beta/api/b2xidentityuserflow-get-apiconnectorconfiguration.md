---
title: Obter userFlowApiConnectorConfiguration
description: Obter a propriedade userFlowApiConnectorConfiguration de um b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 986737621f5b98226c64124f69ac5522c9f5bf69
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843673"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="da813-103">Obter userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="da813-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="da813-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da813-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da813-105">Obter a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) para detalhar os conectores de API habilitados para o fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="da813-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="da813-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="da813-106">Permissions</span></span>

<span data-ttu-id="da813-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da813-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da813-109">Permission type</span></span>      | <span data-ttu-id="da813-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da813-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da813-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da813-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da813-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da813-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="da813-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da813-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="da813-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da813-114">Not supported.</span></span>|
|<span data-ttu-id="da813-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da813-115">Application</span></span>|<span data-ttu-id="da813-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da813-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="da813-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="da813-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="da813-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="da813-118">Global administrator</span></span>
* <span data-ttu-id="da813-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="da813-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="da813-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da813-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da813-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da813-121">Optional query parameters</span></span>

<span data-ttu-id="da813-122">Esse método dá suporte ao `$expand` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da813-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="da813-123">Por exemplo, para recuperar o conector de API e `postFederationSignup` as `postAttributeCollection` etapas, adicione `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="da813-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="da813-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="da813-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="da813-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da813-125">Request headers</span></span>

|<span data-ttu-id="da813-126">Nome</span><span class="sxs-lookup"><span data-stu-id="da813-126">Name</span></span>|<span data-ttu-id="da813-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="da813-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da813-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="da813-128">Authorization</span></span>|<span data-ttu-id="da813-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da813-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da813-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da813-131">Request body</span></span>

<span data-ttu-id="da813-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da813-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da813-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="da813-133">Response</span></span>

<span data-ttu-id="da813-134">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="da813-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="da813-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da813-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da813-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da813-136">Request</span></span>

<span data-ttu-id="da813-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="da813-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="da813-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="da813-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```
# <a name="c"></a>[<span data-ttu-id="da813-139">C#</span><span class="sxs-lookup"><span data-stu-id="da813-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-apiconnectorconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da813-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da813-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-apiconnectorconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da813-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da813-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-apiconnectorconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da813-142">Java</span><span class="sxs-lookup"><span data-stu-id="da813-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-apiconnectorconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da813-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="da813-143">Response</span></span>

<span data-ttu-id="da813-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="da813-144">The following is an example of the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
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
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
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
