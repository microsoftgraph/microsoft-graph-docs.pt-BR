---
title: Listar alertas
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 6036514c2aeabe287fd019ce69157d4b7897af60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860204"
---
# <a name="list-alerts"></a><span data-ttu-id="6b141-104">Listar alertas</span><span class="sxs-lookup"><span data-stu-id="6b141-104">List alerts</span></span>

 > <span data-ttu-id="6b141-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6b141-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b141-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6b141-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b141-107">Recupere uma lista de objetos de [alerta](../resources/alert.md) .</span><span class="sxs-lookup"><span data-stu-id="6b141-107">Retrieve a list of [alert](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b141-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="6b141-108">Permissions</span></span>

<span data-ttu-id="6b141-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b141-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b141-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b141-111">Permission type</span></span>      | <span data-ttu-id="6b141-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b141-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b141-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b141-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b141-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b141-114">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="6b141-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b141-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6b141-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b141-116">Not supported.</span></span>  |
|<span data-ttu-id="6b141-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b141-117">Application</span></span> | <span data-ttu-id="6b141-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b141-118">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b141-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b141-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b141-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b141-120">Optional query parameters</span></span>

<span data-ttu-id="6b141-121">Esse método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="6b141-121">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="6b141-122">`$top`retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="6b141-122">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="6b141-123">Para retornar um conjunto de propriedades alternativo, use o OData `$select` consulta parâmetro para especificar o conjunto de propriedades de **alerta** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="6b141-123">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="6b141-124">Por exemplo, para retornar o **assignedTo**, **categoria**e propriedades de **severidade** , adicione a seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="6b141-124">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

> <span data-ttu-id="6b141-125">**Observação:** `$top` tem um limite de alertas de 1000 e uma combinação de `$top`  +  `$skip` não pode exceder 6000 alertas.</span><span class="sxs-lookup"><span data-stu-id="6b141-125">**Note:** `$top` has a limit of 1000 alerts, and a combination of `$top` + `$skip` cannot exceed 6000 alerts.</span></span> <span data-ttu-id="6b141-126">Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um `200 OK` código de resposta, mas `/security/alerts?$top=10&$skip=5991` retornará um `400 Bad Request` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b141-126">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>  <span data-ttu-id="6b141-127">Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="6b141-127">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b141-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b141-128">Request headers</span></span>

| <span data-ttu-id="6b141-129">Nome</span><span class="sxs-lookup"><span data-stu-id="6b141-129">Name</span></span>      |<span data-ttu-id="6b141-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b141-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6b141-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b141-131">Authorization</span></span>  | <span data-ttu-id="6b141-p106">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b141-p106">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b141-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b141-134">Request body</span></span>

<span data-ttu-id="6b141-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b141-135">Do not supply a request body for this method.</span></span> <span data-ttu-id="6b141-136">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="6b141-136">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6b141-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b141-137">Response</span></span>

<span data-ttu-id="6b141-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de **alerta** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b141-138">If successful, this method returns a `200 OK` response code and collection of **alert** objects in the response body.</span></span> <span data-ttu-id="6b141-139">Se um código de status diferente 2xx ou 404 é retornado por um provedor ou se um provedor de tempo limite, a resposta será um `206 Partial Content` código de status com a resposta do provedor em um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="6b141-139">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="6b141-140">Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="6b141-140">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="6b141-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b141-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b141-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b141-142">Request</span></span>

<span data-ttu-id="6b141-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b141-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/beta/security/alerts
```

### <a name="response"></a><span data-ttu-id="6b141-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b141-144">Response</span></span>

<span data-ttu-id="6b141-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6b141-145">The following is an example of the response.</span></span>

><span data-ttu-id="6b141-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b141-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
