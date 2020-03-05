---
title: Listar alertas
description: Recuperar uma lista de objetos de alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: af59360a3947a98c0bd4cdcbbb826bb014747535
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441611"
---
# <a name="list-alerts"></a><span data-ttu-id="77ffa-103">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="77ffa-103">List alerts</span></span>

<span data-ttu-id="77ffa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77ffa-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77ffa-105">Recuperar uma lista de objetos de [alerta](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="77ffa-105">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="77ffa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77ffa-106">Permissions</span></span>

<span data-ttu-id="77ffa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77ffa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77ffa-109">Permission type</span></span>      | <span data-ttu-id="77ffa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77ffa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77ffa-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77ffa-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="77ffa-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77ffa-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="77ffa-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77ffa-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="77ffa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77ffa-114">Not supported.</span></span>  |
|<span data-ttu-id="77ffa-115">Application</span><span class="sxs-lookup"><span data-stu-id="77ffa-115">Application</span></span> | <span data-ttu-id="77ffa-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77ffa-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77ffa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77ffa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77ffa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77ffa-118">Optional query parameters</span></span>

<span data-ttu-id="77ffa-119">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="77ffa-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="77ffa-120">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="77ffa-120">`$top` will return the aggregated top results from each security API provider.</span></span>

<span data-ttu-id="77ffa-121">Para retornar um conjunto de propriedades alternativas, use o parâmetro de consulta OData `$select` para especificar o conjunto de propriedades de **alerta** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="77ffa-121">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="77ffa-122">Por exemplo, para retornar as propriedades **assignedTo**, **category** e **severity**, adicione o seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="77ffa-122">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="77ffa-123">**Observação:** o parâmetro de consulta OData `$top` tem um limite de 1000 alertas.</span><span class="sxs-lookup"><span data-stu-id="77ffa-123">**Note:** The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="77ffa-124">É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER.</span><span class="sxs-lookup"><span data-stu-id="77ffa-124">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="77ffa-125">Você pode usar `@odata.nextLink` para paginação.</span><span class="sxs-lookup"><span data-stu-id="77ffa-125">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="77ffa-126">Se você precisar usar o `$skip`, ele tem um limite de 500 alertas.</span><span class="sxs-lookup"><span data-stu-id="77ffa-126">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="77ffa-127">Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="77ffa-127">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="77ffa-128">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="77ffa-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="77ffa-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77ffa-129">Request headers</span></span>

| <span data-ttu-id="77ffa-130">Nome</span><span class="sxs-lookup"><span data-stu-id="77ffa-130">Name</span></span>      |<span data-ttu-id="77ffa-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="77ffa-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77ffa-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="77ffa-132">Authorization</span></span>  | <span data-ttu-id="77ffa-133">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="77ffa-133">Bearer {code}.</span></span> <span data-ttu-id="77ffa-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77ffa-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77ffa-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77ffa-135">Request body</span></span>

<span data-ttu-id="77ffa-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77ffa-136">Do not supply a request body for this method.</span></span> <span data-ttu-id="77ffa-137">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="77ffa-137">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="77ffa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="77ffa-138">Response</span></span>

<span data-ttu-id="77ffa-139">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77ffa-139">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="77ffa-140">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="77ffa-140">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="77ffa-141">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="77ffa-141">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="77ffa-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77ffa-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="77ffa-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77ffa-143">Request</span></span>

<span data-ttu-id="77ffa-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77ffa-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77ffa-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="77ffa-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts
```
# <a name="c"></a>[<span data-ttu-id="77ffa-146">C#</span><span class="sxs-lookup"><span data-stu-id="77ffa-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77ffa-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77ffa-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77ffa-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77ffa-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77ffa-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="77ffa-149">Response</span></span>

<span data-ttu-id="77ffa-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77ffa-150">The following is an example of the response.</span></span>

><span data-ttu-id="77ffa-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77ffa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
