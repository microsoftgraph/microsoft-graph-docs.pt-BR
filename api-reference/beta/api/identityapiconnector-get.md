---
title: Obter identityApiConnector
description: Leia as propriedades de um conector de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ce1f12b7ede77d7c9b35b2764fb2ba15825e5c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720085"
---
# <a name="get-identityapiconnector"></a><span data-ttu-id="1c376-103">Obter identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="1c376-103">Get identityApiConnector</span></span>

<span data-ttu-id="1c376-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c376-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c376-105">Ler as propriedades de um objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="1c376-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c376-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c376-106">Permissions</span></span>

<span data-ttu-id="1c376-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c376-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c376-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c376-109">Permission type</span></span>                        | <span data-ttu-id="1c376-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c376-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1c376-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c376-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c376-112">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1c376-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="1c376-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c376-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c376-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c376-114">Not supported.</span></span>  |
| <span data-ttu-id="1c376-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c376-115">Application</span></span>                            | <span data-ttu-id="1c376-116">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1c376-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="1c376-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="1c376-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1c376-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c376-118">Global administrator</span></span>
* <span data-ttu-id="1c376-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="1c376-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1c376-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c376-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c376-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c376-121">Optional query parameters</span></span>
<span data-ttu-id="1c376-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c376-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1c376-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1c376-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c376-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c376-124">Request headers</span></span>
|<span data-ttu-id="1c376-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1c376-125">Name</span></span>|<span data-ttu-id="1c376-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c376-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c376-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c376-127">Authorization</span></span>|<span data-ttu-id="1c376-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c376-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c376-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c376-130">Request body</span></span>
<span data-ttu-id="1c376-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c376-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c376-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c376-132">Response</span></span>

<span data-ttu-id="1c376-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c376-133">If successful, this method returns a `200 OK` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c376-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c376-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c376-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c376-135">Request</span></span>

<span data-ttu-id="1c376-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c376-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityapiconnector"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```

### <a name="response"></a><span data-ttu-id="1c376-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c376-137">Response</span></span>

<span data-ttu-id="1c376-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c376-138">The following is an example of the response.</span></span>

<span data-ttu-id="1c376-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c376-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
