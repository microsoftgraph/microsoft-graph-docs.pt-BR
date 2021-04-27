---
title: Listar alertas
description: Recuperar uma lista de objetos de alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 79d430f7ed898795a8fec07280b5bb30d9400af8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048187"
---
# <a name="list-alerts"></a><span data-ttu-id="91206-103">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="91206-103">List alerts</span></span>

<span data-ttu-id="91206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91206-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91206-105">Recuperar uma lista de objetos de [alerta](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="91206-105">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="91206-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="91206-106">Permissions</span></span>

<span data-ttu-id="91206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91206-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91206-109">Permission type</span></span>      | <span data-ttu-id="91206-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91206-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91206-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91206-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="91206-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91206-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="91206-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91206-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91206-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91206-114">Not supported.</span></span>  |
|<span data-ttu-id="91206-115">Application</span><span class="sxs-lookup"><span data-stu-id="91206-115">Application</span></span> | <span data-ttu-id="91206-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91206-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91206-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91206-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91206-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91206-118">Optional query parameters</span></span>

<span data-ttu-id="91206-119">Este método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="91206-119">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="91206-120">`$top` - Retorna os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="91206-120">`$top` - Returns the aggregated top results from each security API provider.</span></span>
- `$filter`

<span data-ttu-id="91206-121">A tabela a seguir lista as palavras-chave `$filter` para cada nome de fornecedor.</span><span class="sxs-lookup"><span data-stu-id="91206-121">The following table lists the `$filter` keywords by each vendor name.</span></span>

| <span data-ttu-id="91206-122">Anotações do fornecedor</span><span class="sxs-lookup"><span data-stu-id="91206-122">Vendor name</span></span>      |<span data-ttu-id="91206-123">palavra-chave $filter</span><span class="sxs-lookup"><span data-stu-id="91206-123">$filter keyword</span></span>|
|:----------|:----------|
| <span data-ttu-id="91206-124">Proteção Avançada contra Ameaças do Azure</span><span class="sxs-lookup"><span data-stu-id="91206-124">Azure Advanced Threat Protection</span></span> | <span data-ttu-id="91206-125">Proteção Avançada contra Ameaças do Azure</span><span class="sxs-lookup"><span data-stu-id="91206-125">Azure Advanced Threat Protection</span></span> | 
| <span data-ttu-id="91206-126">Central de Segurança do Azure</span><span class="sxs-lookup"><span data-stu-id="91206-126">Azure Security Center</span></span> | <span data-ttu-id="91206-127">ASC</span><span class="sxs-lookup"><span data-stu-id="91206-127">ASC</span></span> |
| <span data-ttu-id="91206-128">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="91206-128">Microsoft Cloud App Security</span></span> | <span data-ttu-id="91206-129">MCAS</span><span class="sxs-lookup"><span data-stu-id="91206-129">MCAS</span></span> |
| <span data-ttu-id="91206-130">Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="91206-130">Azure Active Directory Identity Protection</span></span> | <span data-ttu-id="91206-131">IPC</span><span class="sxs-lookup"><span data-stu-id="91206-131">IPC</span></span> |
| <span data-ttu-id="91206-132">Azure Sentinel</span><span class="sxs-lookup"><span data-stu-id="91206-132">Azure Sentinel</span></span> | <span data-ttu-id="91206-133">Azure Sentinel</span><span class="sxs-lookup"><span data-stu-id="91206-133">Azure Sentinel</span></span> |
| <span data-ttu-id="91206-134">Proteção Avançada contra Ameaças do Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="91206-134">Microsoft Defender Advanced Threat Protection</span></span> | <span data-ttu-id="91206-135">Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="91206-135">Microsoft Defender ATP</span></span> |
| <span data-ttu-id="91206-136">Office 365</span><span class="sxs-lookup"><span data-stu-id="91206-136">Office 365</span></span> |  <span data-ttu-id="91206-137">Não há suporte atualmente.</span><span class="sxs-lookup"><span data-stu-id="91206-137">Not currently supported.</span></span> |

<span data-ttu-id="91206-138">Para retornar um conjunto de propriedades alternativas, use o parâmetro de consulta OData `$select` para especificar o conjunto de propriedades de **alerta** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="91206-138">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="91206-139">Por exemplo, para retornar as propriedades **assignedTo**, **category** e **severity**, adicione o seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="91206-139">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="91206-140">**Observação:** o parâmetro de consulta OData `$top` tem um limite de 1000 alertas.</span><span class="sxs-lookup"><span data-stu-id="91206-140">**Note:** The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="91206-141">É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER.</span><span class="sxs-lookup"><span data-stu-id="91206-141">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="91206-142">Você pode usar `@odata.nextLink` para paginação.</span><span class="sxs-lookup"><span data-stu-id="91206-142">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="91206-143">Se você precisar usar o `$skip`, ele tem um limite de 500 alertas.</span><span class="sxs-lookup"><span data-stu-id="91206-143">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="91206-144">Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="91206-144">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="91206-145">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="91206-145">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="91206-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91206-146">Request headers</span></span>

| <span data-ttu-id="91206-147">Nome</span><span class="sxs-lookup"><span data-stu-id="91206-147">Name</span></span>      |<span data-ttu-id="91206-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="91206-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91206-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="91206-149">Authorization</span></span>  | <span data-ttu-id="91206-150">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="91206-150">Bearer {code}.</span></span> <span data-ttu-id="91206-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91206-151">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91206-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91206-152">Request body</span></span>

<span data-ttu-id="91206-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91206-153">Do not supply a request body for this method.</span></span> <span data-ttu-id="91206-154">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="91206-154">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="91206-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="91206-155">Response</span></span>

<span data-ttu-id="91206-156">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91206-156">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="91206-157">Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um código de status `206 Partial Content` com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="91206-157">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="91206-158">Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="91206-158">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="91206-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91206-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="91206-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91206-160">Request</span></span>

<span data-ttu-id="91206-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91206-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91206-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="91206-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/alerts
```
# <a name="c"></a>[<span data-ttu-id="91206-163">C#</span><span class="sxs-lookup"><span data-stu-id="91206-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-alerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91206-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91206-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-alerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91206-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91206-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-alerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91206-166">Java</span><span class="sxs-lookup"><span data-stu-id="91206-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-alerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91206-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="91206-167">Response</span></span>

<span data-ttu-id="91206-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91206-168">The following is an example of the response.</span></span>

><span data-ttu-id="91206-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="91206-169">**Note:** The response object shown here might be shortened for readability.</span></span>
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


