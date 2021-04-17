---
title: Obter userFlowApiConnectorConfiguration
description: Obter a propriedade userFlowApiConnectorConfiguration de um b2xIdentityUserFlow.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a9bdc99041265edf589a493ef5d83dc51f1c115a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882746"
---
# <a name="get-userflowapiconnectorconfiguration"></a><span data-ttu-id="c5d96-103">Obter userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5d96-103">Get userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="c5d96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5d96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5d96-105">Obter a [propriedade apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) em [um b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) para detalhar os conectores de API habilitados para o fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="c5d96-105">Get the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/userFlowApiConnectorConfiguration.md) to detail the API connectors enabled for the user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5d96-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5d96-106">Permissions</span></span>

<span data-ttu-id="c5d96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5d96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d96-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5d96-109">Permission type</span></span>      | <span data-ttu-id="c5d96-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5d96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d96-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5d96-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c5d96-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d96-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c5d96-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5d96-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c5d96-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5d96-114">Not supported.</span></span>|
|<span data-ttu-id="c5d96-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5d96-115">Application</span></span>|<span data-ttu-id="c5d96-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d96-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c5d96-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c5d96-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c5d96-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c5d96-118">Global administrator</span></span>
* <span data-ttu-id="c5d96-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="c5d96-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c5d96-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5d96-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/apiConnectorConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5d96-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5d96-121">Optional query parameters</span></span>

<span data-ttu-id="c5d96-122">Este método dá suporte ao `$expand` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5d96-122">This method supports the `$expand` OData query parameter to help customize the response.</span></span> <span data-ttu-id="c5d96-123">Por exemplo, para recuperar o conector de API para as `postFederationSignup` etapas `postAttributeCollection` e, adicione `$expand=postFederationSignup,postAttributeCollection` .</span><span class="sxs-lookup"><span data-stu-id="c5d96-123">For example, to retrieve the API connector for the `postFederationSignup` and `postAttributeCollection` steps, add `$expand=postFederationSignup,postAttributeCollection`.</span></span> <span data-ttu-id="c5d96-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c5d96-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5d96-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d96-125">Request headers</span></span>

|<span data-ttu-id="c5d96-126">Nome</span><span class="sxs-lookup"><span data-stu-id="c5d96-126">Name</span></span>|<span data-ttu-id="c5d96-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d96-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c5d96-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5d96-128">Authorization</span></span>|<span data-ttu-id="c5d96-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5d96-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d96-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d96-131">Request body</span></span>

<span data-ttu-id="c5d96-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5d96-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5d96-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d96-133">Response</span></span>

<span data-ttu-id="c5d96-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [apiConnectorConfiguration.](../resources/userflowapiconnectorconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5d96-134">If successful, this method returns a `200 OK` response code and an [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="c5d96-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5d96-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5d96-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d96-136">Request</span></span>

<span data-ttu-id="c5d96-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5d96-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xuserflows-apiconnectorconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection
```

### <a name="response"></a><span data-ttu-id="c5d96-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d96-138">Response</span></span>

<span data-ttu-id="c5d96-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5d96-139">The following is an example of the response.</span></span>

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
