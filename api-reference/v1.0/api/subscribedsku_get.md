# <a name="get-subscribedsku"></a><span data-ttu-id="4f104-101">Obter subscribedSku</span><span class="sxs-lookup"><span data-stu-id="4f104-101">Get subscribedSku</span></span>
<span data-ttu-id="4f104-102">Recupere uma assinatura comercial específica que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="4f104-102">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f104-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f104-103">Permissions</span></span>
<span data-ttu-id="4f104-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="4f104-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f104-106">Permission type</span></span>      | <span data-ttu-id="4f104-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f104-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f104-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f104-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4f104-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f104-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f104-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f104-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f104-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f104-111">Not supported.</span></span>    |
|<span data-ttu-id="4f104-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f104-112">Application</span></span> | <span data-ttu-id="4f104-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f104-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f104-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f104-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f104-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f104-115">Optional query parameters</span></span>
<span data-ttu-id="4f104-116">Esse método **não** tem suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="4f104-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f104-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f104-117">Request headers</span></span>
| <span data-ttu-id="4f104-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4f104-118">Name</span></span>       | <span data-ttu-id="4f104-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f104-119">Type</span></span> | <span data-ttu-id="4f104-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f104-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f104-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f104-121">Authorization</span></span>  | <span data-ttu-id="4f104-122">string</span><span class="sxs-lookup"><span data-stu-id="4f104-122">string</span></span>  | <span data-ttu-id="4f104-p102">&lt;Token&gt; de portador. *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="4f104-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f104-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f104-125">Request body</span></span>
<span data-ttu-id="4f104-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f104-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f104-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f104-127">Response</span></span>

<span data-ttu-id="4f104-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f104-128">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f104-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f104-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f104-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f104-130">Request</span></span>
<span data-ttu-id="4f104-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f104-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="4f104-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f104-132">Response</span></span>
<span data-ttu-id="4f104-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f104-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
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
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
