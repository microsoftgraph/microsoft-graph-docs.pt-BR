---
title: Obter userFlowApiConnectorConfiguration
description: Obter a propriedade userFlowApiConnectorConfiguration de um b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7a7a7e852a1d2addf116c352e762e152078e02ea
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919995"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="ed99f-103">Obter userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed99f-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="ed99f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed99f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed99f-105">Obter a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) para detalhar os conectores de API habilitados para o fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed99f-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed99f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed99f-106">Permissions</span></span>

<span data-ttu-id="ed99f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed99f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed99f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed99f-109">Permission type</span></span>      | <span data-ttu-id="ed99f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed99f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed99f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed99f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed99f-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed99f-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ed99f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed99f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ed99f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed99f-114">Not supported.</span></span>|
|<span data-ttu-id="ed99f-115">Application</span><span class="sxs-lookup"><span data-stu-id="ed99f-115">Application</span></span>|<span data-ttu-id="ed99f-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed99f-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ed99f-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ed99f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ed99f-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ed99f-118">Global administrator</span></span>
* <span data-ttu-id="ed99f-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="ed99f-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ed99f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed99f-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed99f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed99f-121">Optional query parameters</span></span>

<span data-ttu-id="ed99f-122">Este método dá suporte ao `$expand` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed99f-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="ed99f-123">Por exemplo, para recuperar o conector de API para as `postFederationSignup` etapas `postAttributeCollection` e, adicione `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="ed99f-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="ed99f-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ed99f-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed99f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed99f-125">Request headers</span></span>

|<span data-ttu-id="ed99f-126">Nome</span><span class="sxs-lookup"><span data-stu-id="ed99f-126">Name</span></span>|<span data-ttu-id="ed99f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed99f-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed99f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed99f-128">Authorization</span></span>|<span data-ttu-id="ed99f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed99f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed99f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed99f-131">Request body</span></span>

<span data-ttu-id="ed99f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed99f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed99f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed99f-133">Response</span></span>

<span data-ttu-id="ed99f-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed99f-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="ed99f-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed99f-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed99f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed99f-136">Request</span></span>

<span data-ttu-id="ed99f-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed99f-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ed99f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed99f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```
# <a name="c"></a>[<span data-ttu-id="ed99f-139">C#</span><span class="sxs-lookup"><span data-stu-id="ed99f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-apiconnectorconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed99f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed99f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-apiconnectorconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed99f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed99f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-apiconnectorconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed99f-142">Java</span><span class="sxs-lookup"><span data-stu-id="ed99f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-apiconnectorconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed99f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed99f-143">Response</span></span>

<span data-ttu-id="ed99f-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed99f-144">The following is an example of the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration(postFederationSignup(),postAttributeCollection())",
    "postFederationSignup@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postFederationSignup/$entity",
    "postFederationSignup": {
        "id": "74d13179-2c02-4ae7-bff3-82842d4e2f1f",
        "displayName": "Test API Connector 1",
        "targetUrl": "https://someapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "apiAccount",
            "password": "******"
        }
    },
    "postAttributeCollection@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_testuserflow')/apiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/microsoft.graph.userFlowApiConnectorConfiguration/postAttributeCollection/$entity",
    "postAttributeCollection": {
        "id": "900bc92c-bcbf-4093-af8e-450a4a77635f",
        "displayName": "Test API Connector 2",
        "targetUrl": "https://someotherapi.com/api/endpoint",
        "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "apiAccount",
            "password": "******"
        }
    }
}
```
