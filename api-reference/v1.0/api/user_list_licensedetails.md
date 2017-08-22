# <a name="list-licensedetails"></a><span data-ttu-id="334c2-101">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="334c2-101">List licenseDetails</span></span>

<span data-ttu-id="334c2-102">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="334c2-102">Retrieve a list of licenseDetails objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="334c2-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="334c2-103">Prerequisites</span></span>
<span data-ttu-id="334c2-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read*; *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="334c2-104">One of the following **scopes** is required to execute this API: *User.Read*; *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="334c2-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="334c2-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="334c2-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="334c2-106">Optional query parameters</span></span>
<span data-ttu-id="334c2-107">Esse método **não** suporta [Parâmetros da Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="334c2-107">This method does **not** support [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="334c2-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="334c2-108">Request headers</span></span>
| <span data-ttu-id="334c2-109">Nome</span><span class="sxs-lookup"><span data-stu-id="334c2-109">Name</span></span>      |<span data-ttu-id="334c2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="334c2-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="334c2-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="334c2-111">Authorization</span></span>  | <span data-ttu-id="334c2-112">&lt;Código&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="334c2-112">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="334c2-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="334c2-113">Request body</span></span>
<span data-ttu-id="334c2-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="334c2-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="334c2-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="334c2-115">Response</span></span>

<span data-ttu-id="334c2-116">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="334c2-116">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="334c2-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="334c2-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="334c2-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="334c2-118">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="334c2-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="334c2-119">Response</span></span>
<span data-ttu-id="334c2-p101">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="334c2-p101">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->