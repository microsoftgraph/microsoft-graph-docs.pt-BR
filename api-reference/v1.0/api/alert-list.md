---
title: Listar alertas
description: Recupere uma lista de objetos de alerta.
ms.openlocfilehash: c25784f62d37722fc997e57b9f15c9857133b964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006201"
---
# <a name="list-alerts"></a><span data-ttu-id="f48c3-103">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="f48c3-103">List alerts</span></span>

<span data-ttu-id="f48c3-104">Recupere uma lista de objetos de [alerta](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="f48c3-104">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f48c3-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="f48c3-105">Permissions</span></span>

<span data-ttu-id="f48c3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f48c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f48c3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f48c3-108">Permission type</span></span>      | <span data-ttu-id="f48c3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f48c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f48c3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f48c3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f48c3-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48c3-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="f48c3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f48c3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f48c3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f48c3-113">Not supported.</span></span>  |
|<span data-ttu-id="f48c3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f48c3-114">Application</span></span> | <span data-ttu-id="f48c3-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f48c3-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f48c3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f48c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f48c3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f48c3-117">Optional query parameters</span></span>

<span data-ttu-id="f48c3-118">Esse método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="f48c3-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="f48c3-119">`$top`retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="f48c3-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="f48c3-120">Para retornar um conjunto de propriedades alternativo, use o OData `$select` consulta parâmetro para especificar o conjunto de propriedades de **alerta** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="f48c3-120">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="f48c3-121">Por exemplo, para retornar o **assignedTo**, **categoria**e propriedades de **severidade** , adicione a seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="f48c3-121">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f48c3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f48c3-122">Request headers</span></span>

| <span data-ttu-id="f48c3-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f48c3-123">Name</span></span>      |<span data-ttu-id="f48c3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f48c3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f48c3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f48c3-125">Authorization</span></span>  | <span data-ttu-id="f48c3-p103">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f48c3-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f48c3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f48c3-128">Request body</span></span>

<span data-ttu-id="f48c3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f48c3-129">Do not supply a request body for this method.</span></span> <span data-ttu-id="f48c3-130">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="f48c3-130">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="f48c3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f48c3-131">Response</span></span>

<span data-ttu-id="f48c3-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f48c3-132">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="f48c3-133">Se um código de status diferente 2xx ou 404 é retornado por um provedor ou se um provedor de tempo limite, a resposta será um `206 Partial Content` código de status com a resposta de provedores em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="f48c3-133">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the providers response in a warning header.</span></span> <span data-ttu-id="f48c3-134">Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="f48c3-134">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="f48c3-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f48c3-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f48c3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f48c3-136">Request</span></span>

<span data-ttu-id="f48c3-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f48c3-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="f48c3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f48c3-138">Response</span></span>

<span data-ttu-id="f48c3-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f48c3-139">The following is an example of the response.</span></span>

><span data-ttu-id="f48c3-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f48c3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
