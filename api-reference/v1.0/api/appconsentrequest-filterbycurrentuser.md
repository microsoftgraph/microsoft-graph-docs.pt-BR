---
title: 'appConsentRequest: filterByCurrentUser'
description: Recupere appConsentRequests para o qual o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b87e79923b0ea22b9ac32c465885a1f9e259a47f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469503"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="3d35a-103">appConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="3d35a-103">appConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="3d35a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d35a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d35a-105">Recupere [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor e o status do userConsentRequest é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="3d35a-105">Retrieve [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d35a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d35a-106">Permissions</span></span>

<span data-ttu-id="3d35a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d35a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d35a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d35a-109">Permission type</span></span>|<span data-ttu-id="3d35a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d35a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d35a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d35a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d35a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d35a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="3d35a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d35a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d35a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d35a-114">Not supported.</span></span>|
|<span data-ttu-id="3d35a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d35a-115">Application</span></span>|<span data-ttu-id="3d35a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d35a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d35a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d35a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="3d35a-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3d35a-118">Function parameters</span></span>

<span data-ttu-id="3d35a-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="3d35a-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3d35a-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="3d35a-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3d35a-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3d35a-121">Parameter</span></span>|<span data-ttu-id="3d35a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d35a-122">Type</span></span>|<span data-ttu-id="3d35a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d35a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d35a-124">on</span><span class="sxs-lookup"><span data-stu-id="3d35a-124">on</span></span>|<span data-ttu-id="3d35a-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="3d35a-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="3d35a-126">Filtrar para consultar appConsentRequests para o qual o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="3d35a-126">Filter to query appConsentRequests for which the current user is a reviewer.</span></span> <span data-ttu-id="3d35a-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="3d35a-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="3d35a-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d35a-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="3d35a-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d35a-129">Optional query parameters</span></span>

<span data-ttu-id="3d35a-130">Essa função exige que o parâmetro de consulta OData retorne uma  `$filter` coleção de [userConsentRequests](../resources/userconsentrequest.md) para o qual o status é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="3d35a-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequests](../resources/userconsentrequest.md) for which the status is `InProgress`.</span></span> <span data-ttu-id="3d35a-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3d35a-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d35a-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d35a-132">Request headers</span></span>

|<span data-ttu-id="3d35a-133">Nome</span><span class="sxs-lookup"><span data-stu-id="3d35a-133">Name</span></span>|<span data-ttu-id="3d35a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d35a-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d35a-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d35a-135">Authorization</span></span>|<span data-ttu-id="3d35a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d35a-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d35a-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d35a-138">Request body</span></span>

<span data-ttu-id="3d35a-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d35a-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d35a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d35a-140">Response</span></span>

<span data-ttu-id="3d35a-141">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d35a-141">If successful, this function returns a `200 OK` response code and a [appConsentRequest](../resources/appconsentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d35a-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d35a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d35a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d35a-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```

### <a name="response"></a><span data-ttu-id="3d35a-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d35a-144">Response</span></span>

<span data-ttu-id="3d35a-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d35a-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(appConsentRequest)",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

