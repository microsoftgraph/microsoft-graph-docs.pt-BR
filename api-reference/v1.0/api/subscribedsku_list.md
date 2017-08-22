# <a name="list-subscribedskus"></a><span data-ttu-id="313a2-101">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="313a2-101">List subscribedSkus</span></span>
<span data-ttu-id="313a2-102">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="313a2-102">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="313a2-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="313a2-103">Prerequisites</span></span>
<span data-ttu-id="313a2-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="313a2-104">One of the following **scopes** is required to execute this API: *Directory.Read.All*, *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="313a2-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="313a2-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="313a2-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="313a2-106">Optional query parameters</span></span>
<span data-ttu-id="313a2-107">Esse método **não** tem suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="313a2-107">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="313a2-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="313a2-108">Request headers</span></span>
| <span data-ttu-id="313a2-109">Nome</span><span class="sxs-lookup"><span data-stu-id="313a2-109">Name</span></span>       | <span data-ttu-id="313a2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="313a2-110">Type</span></span> | <span data-ttu-id="313a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="313a2-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="313a2-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="313a2-112">Authorization</span></span>  | <span data-ttu-id="313a2-113">string</span><span class="sxs-lookup"><span data-stu-id="313a2-113">string</span></span>  | <span data-ttu-id="313a2-p101">&lt;Token&gt; de portador. *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="313a2-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="313a2-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="313a2-116">Request body</span></span>
<span data-ttu-id="313a2-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="313a2-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="313a2-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="313a2-118">Response</span></span>

<span data-ttu-id="313a2-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="313a2-119">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="313a2-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="313a2-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="313a2-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="313a2-121">Request</span></span>
<span data-ttu-id="313a2-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="313a2-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="313a2-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="313a2-123">Response</span></span>
<span data-ttu-id="313a2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="313a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscribedSkus",
    "value": [
        {
            "capabilityStatus": "Enabled",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
            "prepaidUnits": {
                "enabled": 25,
                "suspended": 0,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
                    "servicePlanName": "ADALLOM_S_O365",
                    "provisioningStatus": "Success",
                    "appliesTo": "User"
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
