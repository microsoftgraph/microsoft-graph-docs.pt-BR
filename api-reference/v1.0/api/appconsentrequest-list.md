---
title: Listar appConsentRequests
description: Recuperar objetos appConsentRequest e suas propriedades
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fba86e4f48a74097cf278fd20c65769f92b959c4
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469498"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="0263d-103">Listar appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="0263d-103">List appConsentRequests</span></span>
<span data-ttu-id="0263d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0263d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0263d-105">Recupere [objetos appConsentRequest](../resources/appconsentrequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0263d-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0263d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0263d-106">Permissions</span></span>

<span data-ttu-id="0263d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0263d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0263d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0263d-109">Permission type</span></span>|<span data-ttu-id="0263d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0263d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0263d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0263d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0263d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0263d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="0263d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0263d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0263d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0263d-114">Not supported.</span></span>|
|<span data-ttu-id="0263d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0263d-115">Application</span></span>|<span data-ttu-id="0263d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="0263d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0263d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0263d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0263d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0263d-118">Optional query parameters</span></span>

<span data-ttu-id="0263d-119">Este método dá suporte aos parâmetros de consulta , , , e OData para  `$select` ajudar a personalizar a `$skip` `$top` `$filter` `$orderby` resposta.</span><span class="sxs-lookup"><span data-stu-id="0263d-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0263d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0263d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0263d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0263d-121">Request headers</span></span>

|<span data-ttu-id="0263d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0263d-122">Name</span></span>|<span data-ttu-id="0263d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0263d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0263d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0263d-124">Authorization</span></span>|<span data-ttu-id="0263d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0263d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0263d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0263d-127">Request body</span></span>

<span data-ttu-id="0263d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0263d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0263d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0263d-129">Response</span></span>

<span data-ttu-id="0263d-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0263d-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0263d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0263d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0263d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0263d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests
```

### <a name="response"></a><span data-ttu-id="0263d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0263d-133">Response</span></span>

<span data-ttu-id="0263d-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0263d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```
