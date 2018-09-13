# <a name="list-alerts"></a><span data-ttu-id="7c9d2-101">List alerts</span><span class="sxs-lookup"><span data-stu-id="7c9d2-101">List alerts</span></span>

<span data-ttu-id="7c9d2-102">Recupera uma lista de objetos [alert](../resources/alert.md).</span><span class="sxs-lookup"><span data-stu-id="7c9d2-102">Retrieve a list of [event](../resources/alert.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c9d2-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c9d2-103">Permissions</span></span>

<span data-ttu-id="7c9d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c9d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c9d2-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c9d2-106">Permission type</span></span>      | <span data-ttu-id="7c9d2-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c9d2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c9d2-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c9d2-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="7c9d2-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9d2-109">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="7c9d2-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c9d2-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7c9d2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-111">Not supported.</span></span>  |
|<span data-ttu-id="7c9d2-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c9d2-112">Application</span></span> | <span data-ttu-id="7c9d2-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9d2-113">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c9d2-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c9d2-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c9d2-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7c9d2-115">Optional query parameters</span></span>

<span data-ttu-id="7c9d2-116">Este método suporta os seguintes [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta:</span><span class="sxs-lookup"><span data-stu-id="7c9d2-116">This method supports the following [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- <span data-ttu-id="7c9d2-117">`$top` retornará os principais resultados agregados de cada provedor de API de segurança.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-117">`$top` will return the aggregated top results from each security API provider.</span></span>  

<span data-ttu-id="7c9d2-118">Para retornar um conjunto alternativo de propriedades, use o parâmetro de consulta OData `$select` para especificar o conjunto de propriedades de **alert** que você deseja.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-118">To return an alternative property set, use the OData `$select` query parameter to specify the set of **alert** properties that you want.</span></span>  <span data-ttu-id="7c9d2-119">Por exemplo, para retornar as propriedades **assignedTo**, **category** e **severity**, adicione o seguinte à sua consulta: `$select=assignedTo,category,severity`.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-119">For example, to return the **assignedTo**, **category**, and **severity** properties, add the following to your query: `$select=assignedTo,category,severity`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c9d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d2-120">Request headers</span></span>

| <span data-ttu-id="7c9d2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7c9d2-121">Name</span></span>      |<span data-ttu-id="7c9d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c9d2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7c9d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c9d2-123">Authorization</span></span>  | <span data-ttu-id="7c9d2-p103">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-p103">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d2-126">Request body</span></span>

<span data-ttu-id="7c9d2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="7c9d2-128">O corpo da solicitação será ignorado.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="7c9d2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c9d2-129">Response</span></span>

<span data-ttu-id="7c9d2-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e a coleção de objetos **alert** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-130">If successful, this method returns a `200 OK` response code and collection of **Attachment** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9d2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c9d2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c9d2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d2-132">Request</span></span>

<span data-ttu-id="7c9d2-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a><span data-ttu-id="7c9d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c9d2-134">Response</span></span>

<span data-ttu-id="7c9d2-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-135">The following is an example of the response.</span></span>

><span data-ttu-id="7c9d2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
