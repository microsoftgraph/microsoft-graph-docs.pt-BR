# <a name="list-photos"></a><span data-ttu-id="f3f67-101">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="f3f67-101">List photos</span></span>

<span data-ttu-id="f3f67-102">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="f3f67-102">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3f67-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3f67-103">Permissions</span></span>
<span data-ttu-id="f3f67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3f67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f3f67-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3f67-106">Permission type</span></span>      | <span data-ttu-id="f3f67-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3f67-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="f3f67-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3f67-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f3f67-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f67-109">Group.Read.All, Group.Readwrite.All</span></span>    | 
|<span data-ttu-id="f3f67-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3f67-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3f67-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3f67-111">Not supported.</span></span>    | 
|<span data-ttu-id="f3f67-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3f67-112">Application</span></span> | <span data-ttu-id="f3f67-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f67-113">Group.Read.All, Group.Readwrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3f67-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3f67-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f3f67-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3f67-115">Optional query parameters</span></span>
<span data-ttu-id="f3f67-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3f67-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3f67-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f67-117">Request headers</span></span>
| <span data-ttu-id="f3f67-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f3f67-118">Name</span></span>       | <span data-ttu-id="f3f67-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3f67-119">Type</span></span> | <span data-ttu-id="f3f67-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3f67-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f3f67-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3f67-121">Authorization</span></span>  | <span data-ttu-id="f3f67-122">string</span><span class="sxs-lookup"><span data-stu-id="f3f67-122">string</span></span>  | <span data-ttu-id="f3f67-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3f67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3f67-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f67-125">Request body</span></span>
<span data-ttu-id="f3f67-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3f67-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3f67-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f67-127">Response</span></span>

<span data-ttu-id="f3f67-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3f67-128">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3f67-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3f67-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3f67-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f67-130">Request</span></span>
<span data-ttu-id="f3f67-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3f67-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```
##### <a name="response"></a><span data-ttu-id="f3f67-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f67-132">Response</span></span>
<span data-ttu-id="f3f67-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3f67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->