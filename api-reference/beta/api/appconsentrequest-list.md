---
title: Listar appConsentRequests
description: Recupere objetos appConsentRequest e suas propriedades.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bab0a202c835c56aaaee1e37a41b1e70d97d3d34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952176"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="0892a-103">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="0892a-103">List appConsentRequests</span></span>
<span data-ttu-id="0892a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0892a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0892a-105">Recupere [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0892a-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0892a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0892a-106">Permissions</span></span>
<span data-ttu-id="0892a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0892a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0892a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0892a-109">Permission type</span></span>|<span data-ttu-id="0892a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0892a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0892a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0892a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0892a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0892a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="0892a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0892a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0892a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0892a-114">Not supported.</span></span>|
|<span data-ttu-id="0892a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0892a-115">Application</span></span>|<span data-ttu-id="0892a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="0892a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0892a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0892a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0892a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0892a-118">Optional query parameters</span></span>
<span data-ttu-id="0892a-119">Este método dá suporte aos parâmetros de consulta , , , e OData para  `$select` ajudar a personalizar a `$skip` `$top` `$filter` `$orderby` resposta.</span><span class="sxs-lookup"><span data-stu-id="0892a-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0892a-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0892a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0892a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0892a-121">Request headers</span></span>
|<span data-ttu-id="0892a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0892a-122">Name</span></span>|<span data-ttu-id="0892a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0892a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0892a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0892a-124">Authorization</span></span>|<span data-ttu-id="0892a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0892a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0892a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0892a-127">Request body</span></span>
<span data-ttu-id="0892a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0892a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0892a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0892a-129">Response</span></span>

<span data-ttu-id="0892a-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0892a-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="example-1-list-all-appconsentrequests"></a><span data-ttu-id="0892a-131">Exemplo 1: Listar todos os appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="0892a-131">Example 1: List all appConsentRequests</span></span>

### <a name="request"></a><span data-ttu-id="0892a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0892a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests
```


### <a name="response"></a><span data-ttu-id="0892a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0892a-133">Response</span></span>
<span data-ttu-id="0892a-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0892a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

## <a name="example-2-list-all-appconsentrequests-with-at-least-one-userconsentrequest-whose-status-is-inprogress"></a><span data-ttu-id="0892a-135">Exemplo 2: listar todos os appConsentRequests com pelo menos um userConsentRequest cujo status é InProgress</span><span class="sxs-lookup"><span data-stu-id="0892a-135">Example 2: List all appConsentRequests with at least one userConsentRequest whose status is InProgress</span></span>

### <a name="request"></a><span data-ttu-id="0892a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0892a-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest_userconsentrequest_InProgress"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests?$filter=userConsentRequests/any (u:u/status eq 'InProgress')
```


### <a name="response"></a><span data-ttu-id="0892a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0892a-137">Response</span></span>
<span data-ttu-id="0892a-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0892a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
    "@odata.count": 1,
    "value": [
      {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

