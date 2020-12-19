---
title: Obter userFlowApiConnectorConfiguration
description: Obtenha a propriedade userFlowApiConnectorConfiguration de um b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59d3e7afb85511abca1575c0a8251811c1e84239
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720043"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="867bc-103">Obter userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="867bc-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="867bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="867bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="867bc-105">Obtenha a propriedade [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em um [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) para detalhar os conectores de API habilitados para o fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="867bc-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="867bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="867bc-106">Permissions</span></span>

<span data-ttu-id="867bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="867bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="867bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="867bc-109">Permission type</span></span>      | <span data-ttu-id="867bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="867bc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="867bc-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="867bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="867bc-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867bc-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="867bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="867bc-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="867bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="867bc-114">Not supported.</span></span>|
|<span data-ttu-id="867bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="867bc-115">Application</span></span>|<span data-ttu-id="867bc-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="867bc-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="867bc-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="867bc-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="867bc-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="867bc-118">Global administrator</span></span>
* <span data-ttu-id="867bc-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="867bc-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="867bc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="867bc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="867bc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="867bc-121">Optional query parameters</span></span>

<span data-ttu-id="867bc-122">Este método oferece suporte ao `$expand` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="867bc-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="867bc-123">Por exemplo, para recuperar o conector de API para o `postFederationSignup` e `postAttributeCollection` as etapas, adicione `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="867bc-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="867bc-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="867bc-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="867bc-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="867bc-125">Request headers</span></span>

|<span data-ttu-id="867bc-126">Nome</span><span class="sxs-lookup"><span data-stu-id="867bc-126">Name</span></span>|<span data-ttu-id="867bc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="867bc-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="867bc-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="867bc-128">Authorization</span></span>|<span data-ttu-id="867bc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="867bc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="867bc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="867bc-131">Request body</span></span>

<span data-ttu-id="867bc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="867bc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="867bc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="867bc-133">Response</span></span>

<span data-ttu-id="867bc-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="867bc-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="867bc-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="867bc-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="867bc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="867bc-136">Request</span></span>

<span data-ttu-id="867bc-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="867bc-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```

### <a name="response"></a><span data-ttu-id="867bc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="867bc-138">Response</span></span>

<span data-ttu-id="867bc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="867bc-139">The following is an example of the response.</span></span>

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
