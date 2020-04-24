---
title: Listar relyingPartyDetailedSummary
description: Recupere uma lista de objetos relyingPartyDetailedSummary.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7edbc02278506a037521031b9db39eadf01efcb9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806134"
---
# <a name="list-relyingpartydetailedsummary"></a><span data-ttu-id="bffce-103">Listar relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="bffce-103">List relyingPartyDetailedSummary</span></span>

<span data-ttu-id="bffce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bffce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bffce-105">Recupere uma lista de objetos **relyingPartyDetailedSummary** .</span><span class="sxs-lookup"><span data-stu-id="bffce-105">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="bffce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bffce-106">Permissions</span></span>

<span data-ttu-id="bffce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bffce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bffce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bffce-109">Permission type</span></span>                        | <span data-ttu-id="bffce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bffce-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bffce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bffce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bffce-112">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="bffce-112">Report.Read.All</span></span> |
| <span data-ttu-id="bffce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bffce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bffce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bffce-114">Not supported.</span></span> |
| <span data-ttu-id="bffce-115">Application</span><span class="sxs-lookup"><span data-stu-id="bffce-115">Application</span></span>                            | <span data-ttu-id="bffce-116">Report. Read. All</span><span class="sxs-lookup"><span data-stu-id="bffce-116">Report.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bffce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bffce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a><span data-ttu-id="bffce-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bffce-118">Function parameters</span></span>

| <span data-ttu-id="bffce-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bffce-119">Parameter</span></span> | <span data-ttu-id="bffce-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bffce-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="bffce-121">ponto</span><span class="sxs-lookup"><span data-stu-id="bffce-121">period</span></span> | <span data-ttu-id="bffce-122">Os valores com suporte são: D1, D7, D30.</span><span class="sxs-lookup"><span data-stu-id="bffce-122">The supported values are: D1, D7, D30.</span></span> <span data-ttu-id="bffce-123">Eles seguem o formato Dn, em que n representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bffce-123">These values follow the format Dn where n represents the number of days over which the report is aggregated.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="bffce-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bffce-124">Optional query parameters</span></span>

<span data-ttu-id="bffce-125">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bffce-125">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="bffce-126">Você pode usar o `$filter` parâmetro para filtrar por RelyingPartyId, migrationStatus e outros atributos.</span><span class="sxs-lookup"><span data-stu-id="bffce-126">You can use the `$filter` parameter to filter by relyingPartyId, migrationStatus and other attributes.</span></span> <span data-ttu-id="bffce-127">Por exemplo, $filter = relyingPartyId EQ ' identifier '.</span><span class="sxs-lookup"><span data-stu-id="bffce-127">For example, $filter= relyingPartyId eq 'identifier'.</span></span>
- <span data-ttu-id="bffce-128">Você pode usar `$orderby`, `$top`e `$skip` parâmetros de consulta em qualquer solicitação get.</span><span class="sxs-lookup"><span data-stu-id="bffce-128">You can use `$orderby`, `$top`, and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="bffce-129">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bffce-129">For general information, see [OData query parameters](/graph/query-parameters).</span></span>


## <a name="request-headers"></a><span data-ttu-id="bffce-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bffce-130">Request headers</span></span>

| <span data-ttu-id="bffce-131">Nome</span><span class="sxs-lookup"><span data-stu-id="bffce-131">Name</span></span>      |<span data-ttu-id="bffce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bffce-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bffce-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="bffce-133">Authorization</span></span> | <span data-ttu-id="bffce-134">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="bffce-134">Bearer {code}.</span></span> <span data-ttu-id="bffce-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bffce-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bffce-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bffce-136">Request body</span></span>

<span data-ttu-id="bffce-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bffce-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bffce-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bffce-138">Response</span></span>

<span data-ttu-id="bffce-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bffce-139">If successful, this method returns a `200 OK` response code and the requested [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bffce-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bffce-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bffce-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bffce-141">Request</span></span>

<span data-ttu-id="bffce-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bffce-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bffce-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bffce-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```
# <a name="c"></a>[<span data-ttu-id="bffce-144">C#</span><span class="sxs-lookup"><span data-stu-id="bffce-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relyingpartydetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bffce-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bffce-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relyingpartydetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bffce-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bffce-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relyingpartydetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bffce-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bffce-147">Response</span></span>

<span data-ttu-id="bffce-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bffce-148">The following is an example of the response.</span></span>

> <span data-ttu-id="bffce-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bffce-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1fec2821-6c43-4919-9560-ce36c820faa5",
  "relyingPartyId": "https://contosoorg-dev-ed.my.contoso.com",
  "serviceId": "287ed092-c182-4748-99a9-9ef3b5a0a0f9",
  "relyingPartyName": "contoso",
  "successfulSignInCount": 90,
  "failedSignInCount": 10,
  "totalSignInCount": 100,
  "signInSuccessRate":90.0,
  "uniqueUserCount": 10,
  "migrationStatus": "ready",
  "replyUrls": [
      "https://contosoorg-dev-ed.my.contoso.com"
  ],
  "migrationValidationDetails": [
      {
          "name": "AdditionalWSFedEndpointCheckResult",
          "value": "{\"result\": 0, \"message\": \"No additional WS-Federation endpoints were found.\"}"
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get relyingPartyDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
