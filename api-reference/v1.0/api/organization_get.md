# <a name="get-organization"></a><span data-ttu-id="96eff-101">Obter organização</span><span class="sxs-lookup"><span data-stu-id="96eff-101">Get organization</span></span>

<span data-ttu-id="96eff-102">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="96eff-102">Retrieve the properties and relationships of currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="96eff-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="96eff-103">Permissions</span></span>
<span data-ttu-id="96eff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="96eff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="96eff-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96eff-106">Permission type</span></span>      | <span data-ttu-id="96eff-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96eff-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96eff-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96eff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="96eff-109">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96eff-109">Not supported.</span></span>    |
|<span data-ttu-id="96eff-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96eff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96eff-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96eff-111">Not supported.</span></span>    |
|<span data-ttu-id="96eff-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96eff-112">Application</span></span> | <span data-ttu-id="96eff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96eff-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96eff-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96eff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization

```
## <a name="optional-query-parameters"></a><span data-ttu-id="96eff-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96eff-115">Optional query parameters</span></span>
<span data-ttu-id="96eff-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96eff-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96eff-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96eff-117">Request headers</span></span>
| <span data-ttu-id="96eff-118">Nome</span><span class="sxs-lookup"><span data-stu-id="96eff-118">Name</span></span>       | <span data-ttu-id="96eff-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="96eff-119">Type</span></span> | <span data-ttu-id="96eff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="96eff-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96eff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96eff-121">Authorization</span></span>  | <span data-ttu-id="96eff-122">string</span><span class="sxs-lookup"><span data-stu-id="96eff-122">string</span></span>  | <span data-ttu-id="96eff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96eff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96eff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96eff-125">Request body</span></span>
<span data-ttu-id="96eff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96eff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96eff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="96eff-127">Response</span></span>

<span data-ttu-id="96eff-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96eff-128">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96eff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96eff-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96eff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96eff-130">Request</span></span>
<span data-ttu-id="96eff-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96eff-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="96eff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="96eff-132">Response</span></span>
<span data-ttu-id="96eff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96eff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->