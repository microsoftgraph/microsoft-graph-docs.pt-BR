---
title: Obter identityApiConnector
description: Leia as propriedades de um conector de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52acb028462d83c6cf555659fbada6234eb90363
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882769"
---
# <a name="get-identityapiconnector"></a><span data-ttu-id="ab126-103">Obter identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ab126-103">Get identityApiConnector</span></span>

<span data-ttu-id="ab126-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab126-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab126-105">Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ab126-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab126-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab126-106">Permissions</span></span>

<span data-ttu-id="ab126-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab126-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab126-109">Permission type</span></span>                        | <span data-ttu-id="ab126-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab126-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ab126-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab126-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab126-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab126-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="ab126-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab126-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab126-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab126-114">Not supported.</span></span>  |
| <span data-ttu-id="ab126-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab126-115">Application</span></span>                            | <span data-ttu-id="ab126-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab126-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="ab126-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ab126-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ab126-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ab126-118">Global administrator</span></span>
* <span data-ttu-id="ab126-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="ab126-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ab126-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab126-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab126-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab126-121">Optional query parameters</span></span>

<span data-ttu-id="ab126-122">Você pode usar `$expand` para expandir propriedades específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="ab126-122">You can use `$expand` to expand specific properties that are not expanded by default.</span></span> <span data-ttu-id="ab126-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab126-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab126-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab126-124">Request headers</span></span>

|<span data-ttu-id="ab126-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ab126-125">Name</span></span>|<span data-ttu-id="ab126-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab126-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ab126-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab126-127">Authorization</span></span>|<span data-ttu-id="ab126-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab126-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab126-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab126-130">Request body</span></span>

<span data-ttu-id="ab126-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab126-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab126-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab126-132">Response</span></span>

<span data-ttu-id="ab126-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab126-133">If successful, this method returns a `200 OK` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab126-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab126-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab126-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab126-135">Request</span></span>

<span data-ttu-id="ab126-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab126-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```

### <a name="response"></a><span data-ttu-id="ab126-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab126-137">Response</span></span>

<span data-ttu-id="ab126-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab126-138">The following is an example of the response.</span></span>

<span data-ttu-id="ab126-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab126-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"370eeb68-dfd3-4a47-8160-8824c2358321",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
