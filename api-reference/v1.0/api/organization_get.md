# <a name="get-organization"></a><span data-ttu-id="127fe-101">Obter organização</span><span class="sxs-lookup"><span data-stu-id="127fe-101">Get organization</span></span>

<span data-ttu-id="127fe-102">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="127fe-102">Retrieve the properties and relationships of currently authenticated organization.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="127fe-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="127fe-103">Prerequisites</span></span>
<span data-ttu-id="127fe-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="127fe-104">One of the following **scopes** is required to execute this API:</span></span> 
## <a name="http-request"></a><span data-ttu-id="127fe-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="127fe-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization

```
## <a name="optional-query-parameters"></a><span data-ttu-id="127fe-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="127fe-106">Optional query parameters</span></span>
<span data-ttu-id="127fe-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="127fe-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="127fe-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="127fe-108">Request headers</span></span>
| <span data-ttu-id="127fe-109">Nome</span><span class="sxs-lookup"><span data-stu-id="127fe-109">Name</span></span>       | <span data-ttu-id="127fe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="127fe-110">Type</span></span> | <span data-ttu-id="127fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="127fe-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="127fe-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="127fe-112">Authorization</span></span>  | <span data-ttu-id="127fe-113">string</span><span class="sxs-lookup"><span data-stu-id="127fe-113">string</span></span>  | <span data-ttu-id="127fe-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="127fe-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="127fe-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="127fe-116">Request body</span></span>
<span data-ttu-id="127fe-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="127fe-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="127fe-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="127fe-118">Response</span></span>

<span data-ttu-id="127fe-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="127fe-119">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="127fe-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="127fe-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="127fe-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="127fe-121">Request</span></span>
<span data-ttu-id="127fe-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="127fe-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/v1.0/organization
```
##### <a name="response"></a><span data-ttu-id="127fe-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="127fe-123">Response</span></span>
<span data-ttu-id="127fe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="127fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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