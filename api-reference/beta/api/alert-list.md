---
title: Listar alertas
description: Recuperar uma lista de objetos de alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6a40c56ce0caf372ffdb40bb73cac468b0de0523
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318819"
---
# <a name="list-alerts"></a><span data-ttu-id="578b4-103">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="578b4-103">List alerts</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="578b4-104">Recuperar uma lista de objetos de [alerta](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="578b4-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="578b4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="578b4-105">Permissions</span></span>

<span data-ttu-id="578b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="578b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="578b4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="578b4-108">Permission type</span></span>      | <span data-ttu-id="578b4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="578b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="578b4-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="578b4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="578b4-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578b4-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="578b4-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="578b4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="578b4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="578b4-113">Not supported.</span></span>  |
|<span data-ttu-id="578b4-114">Application</span><span class="sxs-lookup"><span data-stu-id="578b4-114">Application</span></span> | <span data-ttu-id="578b4-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578b4-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="578b4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="578b4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="578b4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="578b4-117">Optional query parameters</span></span>

<span data-ttu-id="578b4-118">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="578b4-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="578b4-119">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="578b4-119">`$top` will return the aggregated top results from each security API provider.</span></span>

<span data-ttu-id="578b4-120">Para retornar um conjunto de propriedades alternativas, use o parâmetro de consulta OData `$select` para especificar o conjunto de propriedades de **alerta** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="578b4-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="578b4-121">Por exemplo, para retornar as propriedades **assignedTo**, **category** e **severity**, adicione o seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="578b4-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="578b4-122">**Observação:** `$top` possui um limite de 1000 alertas, e uma combinação de `$top` + `$skip` não pode exceder 6000 alertas.</span><span class="sxs-lookup"><span data-stu-id="578b4-122">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="578b4-123">Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=5991` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="578b4-123">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="578b4-124">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="578b4-124">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="578b4-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="578b4-125">Request headers</span></span>

| <span data-ttu-id="578b4-126">Nome</span><span class="sxs-lookup"><span data-stu-id="578b4-126">Name</span></span>      |<span data-ttu-id="578b4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="578b4-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="578b4-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="578b4-128">Authorization</span></span>  | <span data-ttu-id="578b4-129">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="578b4-129">Bearer {code}.</span></span> <span data-ttu-id="578b4-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="578b4-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="578b4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="578b4-131">Request body</span></span>

<span data-ttu-id="578b4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="578b4-132">Do not supply a request body for this method.</span></span> <span data-ttu-id="578b4-133">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="578b4-133">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="578b4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="578b4-134">Response</span></span>

<span data-ttu-id="578b4-135">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="578b4-135">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="578b4-136">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="578b4-136">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="578b4-137">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="578b4-137">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="578b4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="578b4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="578b4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="578b4-139">Request</span></span>

<span data-ttu-id="578b4-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="578b4-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="578b4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="578b4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="578b4-142">C#</span><span class="sxs-lookup"><span data-stu-id="578b4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="578b4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="578b4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="578b4-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="578b4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="578b4-145">Java</span><span class="sxs-lookup"><span data-stu-id="578b4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="578b4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="578b4-146">Response</span></span>

<span data-ttu-id="578b4-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="578b4-147">The following is an example of the response.</span></span>

><span data-ttu-id="578b4-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="578b4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
