# <a name="list-subscribedskus"></a><span data-ttu-id="64d0e-101">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="64d0e-101">List subscribedSkus</span></span>
<span data-ttu-id="64d0e-102">Recupere a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="64d0e-102">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="64d0e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="64d0e-103">Permissions</span></span>
<span data-ttu-id="64d0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64d0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="64d0e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64d0e-106">Permission type</span></span>      | <span data-ttu-id="64d0e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64d0e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64d0e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64d0e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="64d0e-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64d0e-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64d0e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64d0e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64d0e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64d0e-111">Not supported.</span></span>    |
|<span data-ttu-id="64d0e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64d0e-112">Application</span></span> | <span data-ttu-id="64d0e-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d0e-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64d0e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64d0e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64d0e-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64d0e-115">Optional query parameters</span></span>
<span data-ttu-id="64d0e-116">Esse método **não** tem suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="64d0e-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64d0e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64d0e-117">Request headers</span></span>
| <span data-ttu-id="64d0e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="64d0e-118">Name</span></span>       | <span data-ttu-id="64d0e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="64d0e-119">Type</span></span> | <span data-ttu-id="64d0e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="64d0e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64d0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="64d0e-121">Authorization</span></span>  | <span data-ttu-id="64d0e-122">string</span><span class="sxs-lookup"><span data-stu-id="64d0e-122">string</span></span>  | <span data-ttu-id="64d0e-p102">&lt;Token&gt; de portador. *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="64d0e-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="64d0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64d0e-125">Request body</span></span>
<span data-ttu-id="64d0e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64d0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64d0e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64d0e-127">Response</span></span>

<span data-ttu-id="64d0e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64d0e-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64d0e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64d0e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64d0e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64d0e-130">Request</span></span>
<span data-ttu-id="64d0e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64d0e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="64d0e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="64d0e-132">Response</span></span>
<span data-ttu-id="64d0e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64d0e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
