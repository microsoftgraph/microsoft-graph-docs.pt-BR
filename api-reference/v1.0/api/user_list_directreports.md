# <a name="list-directreports"></a><span data-ttu-id="a2f5a-101">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="a2f5a-101">List directReports</span></span>

<span data-ttu-id="a2f5a-p101">Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2f5a-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2f5a-104">Prerequisites</span></span>
<span data-ttu-id="a2f5a-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="a2f5a-105">One of the following **scopes** is required to execute this API: *User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="a2f5a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2f5a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a2f5a-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a2f5a-107">Optional query parameters</span></span>
<span data-ttu-id="a2f5a-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2f5a-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f5a-109">Request headers</span></span>
| <span data-ttu-id="a2f5a-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2f5a-110">Header</span></span>       | <span data-ttu-id="a2f5a-111">Valor</span><span class="sxs-lookup"><span data-stu-id="a2f5a-111">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a2f5a-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2f5a-112">Authorization</span></span>  | <span data-ttu-id="a2f5a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a2f5a-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2f5a-115">Content-Type</span></span>   | <span data-ttu-id="a2f5a-116">application/json</span><span class="sxs-lookup"><span data-stu-id="a2f5a-116">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="a2f5a-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f5a-117">Request body</span></span>
<span data-ttu-id="a2f5a-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2f5a-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2f5a-119">Response</span></span>

<span data-ttu-id="a2f5a-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-120">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a2f5a-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2f5a-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2f5a-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2f5a-122">Request</span></span>
<span data-ttu-id="a2f5a-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="a2f5a-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2f5a-124">Response</span></span>
<span data-ttu-id="a2f5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2f5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->