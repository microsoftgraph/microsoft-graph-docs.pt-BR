# <a name="list-createdobjects"></a><span data-ttu-id="88244-101">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="88244-101">List createdObjects</span></span>

<span data-ttu-id="88244-102">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="88244-102">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="88244-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="88244-103">Permissions</span></span>
<span data-ttu-id="88244-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88244-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88244-106">Permission type</span></span>      | <span data-ttu-id="88244-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88244-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88244-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88244-108">Delegated (work or school account)</span></span> | <span data-ttu-id="88244-109">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88244-109">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88244-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88244-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88244-111">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88244-111">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="88244-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88244-112">Application</span></span> | <span data-ttu-id="88244-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88244-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88244-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88244-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88244-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="88244-115">Optional query parameters</span></span>
<span data-ttu-id="88244-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="88244-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="88244-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88244-117">Request headers</span></span>
| <span data-ttu-id="88244-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88244-118">Header</span></span>       | <span data-ttu-id="88244-119">Valor</span><span class="sxs-lookup"><span data-stu-id="88244-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88244-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="88244-120">Authorization</span></span>  | <span data-ttu-id="88244-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88244-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88244-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88244-123">Content-Type</span></span>  | <span data-ttu-id="88244-124">application/json</span><span class="sxs-lookup"><span data-stu-id="88244-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88244-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88244-125">Request body</span></span>
<span data-ttu-id="88244-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88244-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88244-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="88244-127">Response</span></span>

<span data-ttu-id="88244-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88244-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88244-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88244-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88244-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88244-130">Request</span></span>
<span data-ttu-id="88244-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88244-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="88244-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="88244-132">Response</span></span>
<span data-ttu-id="88244-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88244-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->