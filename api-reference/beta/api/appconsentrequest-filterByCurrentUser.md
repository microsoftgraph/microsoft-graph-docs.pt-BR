---
title: 'appConsentRequests: filterByCurrentUser'
description: Recupere appConsentRequests para o qual o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f2b615082d38460ec32a7e479aa76ef771c87b36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952178"
---
# <a name="appconsentrequests-filterbycurrentuser"></a><span data-ttu-id="37a0c-103">appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="37a0c-103">appConsentRequests: filterByCurrentUser</span></span>
<span data-ttu-id="37a0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a0c-105">Recupere [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor e o status do userConsentRequest é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="37a0c-105">Retrieve [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="37a0c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37a0c-106">Permissions</span></span>
<span data-ttu-id="37a0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a0c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a0c-109">Permission type</span></span>|<span data-ttu-id="37a0c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37a0c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a0c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37a0c-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a0c-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="37a0c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a0c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37a0c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a0c-114">Not supported.</span></span>|
|<span data-ttu-id="37a0c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a0c-115">Application</span></span>|<span data-ttu-id="37a0c-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a0c-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37a0c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a0c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="37a0c-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="37a0c-118">Function parameters</span></span>
<span data-ttu-id="37a0c-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="37a0c-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="37a0c-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="37a0c-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="37a0c-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37a0c-121">Property</span></span>|<span data-ttu-id="37a0c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="37a0c-122">Type</span></span>|<span data-ttu-id="37a0c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a0c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a0c-124">on</span><span class="sxs-lookup"><span data-stu-id="37a0c-124">on</span></span>|<span data-ttu-id="37a0c-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="37a0c-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="37a0c-126">Filtrar para consultar appConsentRequests para o qual o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="37a0c-126">Filter to query appConsentRequests for which the current user is a reviewer.</span></span> <span data-ttu-id="37a0c-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="37a0c-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="37a0c-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a0c-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="37a0c-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37a0c-129">Optional query parameters</span></span>
<span data-ttu-id="37a0c-130">Essa função requer o parâmetro de consulta OData para retornar uma  `$filter` coleção de [userConsentRequests](../resources/userconsentrequest.md) cujo status é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="37a0c-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequests](../resources/userconsentrequest.md) whose status is `InProgress`.</span></span> <span data-ttu-id="37a0c-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37a0c-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a0c-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a0c-132">Request headers</span></span>
|<span data-ttu-id="37a0c-133">Nome</span><span class="sxs-lookup"><span data-stu-id="37a0c-133">Name</span></span>|<span data-ttu-id="37a0c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a0c-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37a0c-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a0c-135">Authorization</span></span>|<span data-ttu-id="37a0c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a0c-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a0c-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37a0c-138">Request body</span></span>
<span data-ttu-id="37a0c-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37a0c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a0c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a0c-140">Response</span></span>

<span data-ttu-id="37a0c-141">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a0c-141">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a0c-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37a0c-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37a0c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a0c-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```


### <a name="response"></a><span data-ttu-id="37a0c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a0c-144">Response</span></span>
<span data-ttu-id="37a0c-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37a0c-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(appConsentRequest)",
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

