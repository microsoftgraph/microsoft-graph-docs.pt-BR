---
title: 'appConsentRequests: filterByCurrentUser'
description: Recupere appConsentRequests para o qual o usuário atual é o revistor.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2fa7c1c345abe68c0fd2af2d588f07d00468e462
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201741"
---
# <a name="appconsentrequests-filterbycurrentuser"></a><span data-ttu-id="7a959-103">appConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="7a959-103">appConsentRequests: filterByCurrentUser</span></span>
<span data-ttu-id="7a959-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a959-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a959-105">Recupere [appConsentRequests](../resources/appconsentrequest.md) para o qual o usuário atual é o revistor e o status do userConsentRequest é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="7a959-105">Retrieve [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a959-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a959-106">Permissions</span></span>
<span data-ttu-id="7a959-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a959-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a959-109">Permission type</span></span>|<span data-ttu-id="7a959-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a959-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a959-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a959-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a959-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a959-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="7a959-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a959-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a959-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a959-114">Not supported.</span></span>|
|<span data-ttu-id="7a959-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a959-115">Application</span></span>|<span data-ttu-id="7a959-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a959-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a959-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a959-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="7a959-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7a959-118">Function parameters</span></span>
<span data-ttu-id="7a959-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="7a959-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7a959-120">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="7a959-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7a959-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a959-121">Property</span></span>|<span data-ttu-id="7a959-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a959-122">Type</span></span>|<span data-ttu-id="7a959-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a959-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a959-124">on</span><span class="sxs-lookup"><span data-stu-id="7a959-124">on</span></span>|<span data-ttu-id="7a959-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="7a959-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="7a959-126">Filtrar para consultar appConsentRequests para o qual o usuário atual é um revistor.</span><span class="sxs-lookup"><span data-stu-id="7a959-126">Filter to query appConsentRequests for which the current user is a reviewer.</span></span> <span data-ttu-id="7a959-127">O valor permitido é `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="7a959-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="7a959-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a959-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="7a959-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a959-129">Optional query parameters</span></span>
<span data-ttu-id="7a959-130">Essa função requer o parâmetro de consulta OData para retornar uma  `$filter` coleção de [userConsentRequests](../resources/userconsentrequest.md) cujo status é `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="7a959-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequests](../resources/userconsentrequest.md) whose status is `InProgress`.</span></span> <span data-ttu-id="7a959-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a959-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a959-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a959-132">Request headers</span></span>
|<span data-ttu-id="7a959-133">Nome</span><span class="sxs-lookup"><span data-stu-id="7a959-133">Name</span></span>|<span data-ttu-id="7a959-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a959-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a959-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a959-135">Authorization</span></span>|<span data-ttu-id="7a959-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a959-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a959-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a959-138">Request body</span></span>
<span data-ttu-id="7a959-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a959-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a959-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a959-140">Response</span></span>

<span data-ttu-id="7a959-141">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos appConsentRequest](../resources/appconsentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a959-141">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a959-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a959-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a959-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a959-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a959-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a959-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="7a959-145">C#</span><span class="sxs-lookup"><span data-stu-id="7a959-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/appconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a959-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a959-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/appconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a959-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a959-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/appconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a959-148">Java</span><span class="sxs-lookup"><span data-stu-id="7a959-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/appconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7a959-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a959-149">Response</span></span>
<span data-ttu-id="7a959-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a959-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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

