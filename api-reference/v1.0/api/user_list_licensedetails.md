# <a name="list-licensedetails"></a><span data-ttu-id="f32b5-101">Listar licenseDetails</span><span class="sxs-lookup"><span data-stu-id="f32b5-101">List licenseDetails</span></span>

<span data-ttu-id="f32b5-102">Recupere uma lista de objetos licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="f32b5-102">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f32b5-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f32b5-103">Permissions</span></span>
<span data-ttu-id="f32b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f32b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f32b5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f32b5-106">Permission type</span></span>      | <span data-ttu-id="f32b5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f32b5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f32b5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f32b5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f32b5-109">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f32b5-109">One of the following scopes is required to execute this API: User.Read; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f32b5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f32b5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f32b5-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="f32b5-111">User.Read</span></span>    |
|<span data-ttu-id="f32b5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f32b5-112">Application</span></span> | <span data-ttu-id="f32b5-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32b5-113">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f32b5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f32b5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f32b5-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f32b5-115">Optional query parameters</span></span>
<span data-ttu-id="f32b5-116">Esse método **não** suporta [Parâmetros da Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="f32b5-116">This method does **not** support [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f32b5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b5-117">Request headers</span></span>
| <span data-ttu-id="f32b5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f32b5-118">Name</span></span>      |<span data-ttu-id="f32b5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f32b5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f32b5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f32b5-120">Authorization</span></span>  | <span data-ttu-id="f32b5-121">&lt;Código&gt; de portador</span><span class="sxs-lookup"><span data-stu-id="f32b5-121">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32b5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b5-122">Request body</span></span>
<span data-ttu-id="f32b5-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f32b5-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f32b5-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32b5-124">Response</span></span>

<span data-ttu-id="f32b5-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [licenseDetails](../resources/licensedetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f32b5-125">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f32b5-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f32b5-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f32b5-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f32b5-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="f32b5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f32b5-128">Response</span></span>
<span data-ttu-id="f32b5-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f32b5-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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