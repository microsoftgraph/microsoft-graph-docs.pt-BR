---
title: Listar relyingPartyDetailedSummary
description: Recupere uma lista de objetos relyingPartyDetailedSummary.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 17e4c4b3e92173593c768267f6db957942241cdf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052856"
---
# <a name="list-relyingpartydetailedsummary"></a><span data-ttu-id="0dcbe-103">Listar relyingPartyDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="0dcbe-103">List relyingPartyDetailedSummary</span></span>

<span data-ttu-id="0dcbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dcbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dcbe-105">Recupere uma lista **de objetos relyingPartyDetailedSummary.**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-105">Retrieve a list of **relyingPartyDetailedSummary** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dcbe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0dcbe-106">Permissions</span></span>

<span data-ttu-id="0dcbe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dcbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0dcbe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dcbe-109">Permission type</span></span>                        | <span data-ttu-id="0dcbe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0dcbe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dcbe-112">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dcbe-112">Report.Read.All</span></span> |
| <span data-ttu-id="0dcbe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dcbe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-114">Not supported.</span></span> |
| <span data-ttu-id="0dcbe-115">Application</span><span class="sxs-lookup"><span data-stu-id="0dcbe-115">Application</span></span>                            | <span data-ttu-id="0dcbe-116">Report.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dcbe-116">Report.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dcbe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dcbe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getRelyingPartyDetailedSummary
```
## <a name="function-parameters"></a><span data-ttu-id="0dcbe-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="0dcbe-118">Function parameters</span></span>

| <span data-ttu-id="0dcbe-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0dcbe-119">Parameter</span></span> | <span data-ttu-id="0dcbe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcbe-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0dcbe-121">ponto</span><span class="sxs-lookup"><span data-stu-id="0dcbe-121">period</span></span> | <span data-ttu-id="0dcbe-122">Os valores suportados são: D1, D7, D30.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-122">The supported values are: D1, D7, D30.</span></span> <span data-ttu-id="0dcbe-123">Eles seguem o formato Dn, em que n representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-123">These values follow the format Dn where n represents the number of days over which the report is aggregated.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="0dcbe-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0dcbe-124">Optional query parameters</span></span>

<span data-ttu-id="0dcbe-125">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-125">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="0dcbe-126">Você pode usar o `$filter` parâmetro para filtrar confiandoPartyId, migrationStatus e outros atributos.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-126">You can use the `$filter` parameter to filter by relyingPartyId, migrationStatus and other attributes.</span></span> <span data-ttu-id="0dcbe-127">Por exemplo, $filter= relyingPartyId eq 'identifier'.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-127">For example, $filter= relyingPartyId eq 'identifier'.</span></span>
- <span data-ttu-id="0dcbe-128">Você pode usar `$orderby` parâmetros `$top` , e consulta em `$skip` qualquer solicitação GET.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-128">You can use `$orderby`, `$top`, and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="0dcbe-129">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0dcbe-129">For general information, see [OData query parameters](/graph/query-parameters).</span></span>


## <a name="request-headers"></a><span data-ttu-id="0dcbe-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcbe-130">Request headers</span></span>

| <span data-ttu-id="0dcbe-131">Nome</span><span class="sxs-lookup"><span data-stu-id="0dcbe-131">Name</span></span>      |<span data-ttu-id="0dcbe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcbe-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0dcbe-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dcbe-133">Authorization</span></span> | <span data-ttu-id="0dcbe-134">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-134">Bearer {code}.</span></span> <span data-ttu-id="0dcbe-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dcbe-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcbe-136">Request body</span></span>

<span data-ttu-id="0dcbe-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dcbe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dcbe-138">Response</span></span>

<span data-ttu-id="0dcbe-139">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-139">If successful, this method returns a `200 OK` response code and the requested [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0dcbe-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0dcbe-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0dcbe-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dcbe-141">Request</span></span>

<span data-ttu-id="0dcbe-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0dcbe-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dcbe-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getRelyingPartyDetailedSummary(period='period_value')
```
# <a name="c"></a>[<span data-ttu-id="0dcbe-144">C#</span><span class="sxs-lookup"><span data-stu-id="0dcbe-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relyingpartydetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dcbe-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dcbe-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relyingpartydetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dcbe-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dcbe-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relyingpartydetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0dcbe-147">Java</span><span class="sxs-lookup"><span data-stu-id="0dcbe-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-relyingpartydetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0dcbe-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dcbe-148">Response</span></span>

<span data-ttu-id="0dcbe-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-149">The following is an example of the response.</span></span>

> <span data-ttu-id="0dcbe-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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


