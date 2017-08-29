# <a name="list-manager"></a><span data-ttu-id="a9e01-101">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="a9e01-101">List manager</span></span>

<span data-ttu-id="a9e01-p101">Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9e01-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9e01-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9e01-104">Permissions</span></span>
<span data-ttu-id="a9e01-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9e01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9e01-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9e01-107">Permission type</span></span>      | <span data-ttu-id="a9e01-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9e01-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9e01-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9e01-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a9e01-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9e01-110">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9e01-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9e01-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9e01-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9e01-112">Not supported.</span></span>    |
|<span data-ttu-id="a9e01-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9e01-113">Application</span></span> | <span data-ttu-id="a9e01-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e01-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9e01-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9e01-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9e01-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9e01-116">Optional query parameters</span></span>
<span data-ttu-id="a9e01-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9e01-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a9e01-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e01-118">Request headers</span></span>
| <span data-ttu-id="a9e01-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9e01-119">Header</span></span>       | <span data-ttu-id="a9e01-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9e01-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a9e01-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9e01-121">Authorization</span></span>  | <span data-ttu-id="a9e01-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9e01-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a9e01-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9e01-124">Content-Type</span></span>   | <span data-ttu-id="a9e01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9e01-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9e01-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e01-126">Request body</span></span>
<span data-ttu-id="a9e01-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9e01-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9e01-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e01-128">Response</span></span>

<span data-ttu-id="a9e01-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9e01-129">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9e01-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9e01-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9e01-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9e01-131">Request</span></span>
<span data-ttu-id="a9e01-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9e01-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="a9e01-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9e01-133">Response</span></span>
<span data-ttu-id="a9e01-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9e01-134">Here is an example of the response.</span></span>
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
