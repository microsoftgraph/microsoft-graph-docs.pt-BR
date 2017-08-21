# <a name="list-manager"></a><span data-ttu-id="bd4fa-101">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="bd4fa-101">List manager</span></span>

<span data-ttu-id="bd4fa-p101">Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd4fa-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd4fa-104">Prerequisites</span></span>
<span data-ttu-id="bd4fa-105">Um dos seguintes **escopos** é necessário para executar esta API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="bd4fa-105">One of the following **scopes** is required to execute this API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="bd4fa-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd4fa-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd4fa-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd4fa-107">Optional query parameters</span></span>
<span data-ttu-id="bd4fa-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bd4fa-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4fa-109">Request headers</span></span>
| <span data-ttu-id="bd4fa-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd4fa-110">Header</span></span>       | <span data-ttu-id="bd4fa-111">Valor</span><span class="sxs-lookup"><span data-stu-id="bd4fa-111">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="bd4fa-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd4fa-112">Authorization</span></span>  | <span data-ttu-id="bd4fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd4fa-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd4fa-115">Content-Type</span></span>   | <span data-ttu-id="bd4fa-116">application/json</span><span class="sxs-lookup"><span data-stu-id="bd4fa-116">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="bd4fa-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4fa-117">Request body</span></span>
<span data-ttu-id="bd4fa-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd4fa-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd4fa-119">Response</span></span>

<span data-ttu-id="bd4fa-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bd4fa-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd4fa-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd4fa-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd4fa-122">Request</span></span>
<span data-ttu-id="bd4fa-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="bd4fa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd4fa-124">Response</span></span>
<span data-ttu-id="bd4fa-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
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
