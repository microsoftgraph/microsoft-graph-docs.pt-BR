# <a name="list-available-drives"></a><span data-ttu-id="2e4c5-101">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="2e4c5-101">List available drives</span></span>

<span data-ttu-id="2e4c5-p101">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um [User](../resources/user.md) ou [Group](../resources/group.md) de destino. Seu aplicativo também pode solicitar o conjunto de bibliotecas de documentos no site raiz do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-p101">Retrieve the list of [Drive](../resources/drive.md) resources available for a target [User](../resources/user.md) or [Group](../resources/group.md). Your app can also request the set of document libraries on the SharePoint root site.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e4c5-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e4c5-104">Permissions</span></span>

<span data-ttu-id="2e4c5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e4c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e4c5-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e4c5-107">Permission type</span></span>      | <span data-ttu-id="2e4c5-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e4c5-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2e4c5-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e4c5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2e4c5-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4c5-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="2e4c5-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e4c5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e4c5-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4c5-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="2e4c5-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e4c5-113">Application</span></span> | <span data-ttu-id="2e4c5-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4c5-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e4c5-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4c5-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives
GET /me/drives
GET /sites/{site-id}/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e4c5-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2e4c5-116">Optional query parameters</span></span>

<span data-ttu-id="2e4c5-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="2e4c5-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4c5-118">Request body</span></span>

<span data-ttu-id="2e4c5-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e4c5-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4c5-120">Response</span></span>

<span data-ttu-id="2e4c5-121">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-121">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4c5-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e4c5-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e4c5-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4c5-123">Request</span></span>

<span data-ttu-id="2e4c5-124">Eis um exemplo da solicitação de unidades do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-124">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drives"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drives
```

##### <a name="response"></a><span data-ttu-id="2e4c5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4c5-125">Response</span></span>

<span data-ttu-id="2e4c5-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 579

{
  "value": [
    {
      "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
      "driveType": "business",
      "owner": {
          "user": {
              "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
              "displayName": "Ryan Gregg"
          }
      },
      "quota": {
          "deleted": 256938,
          "remaining": 1099447353539,
          "state": "normal",
          "total": 1099511627776
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="2e4c5-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e4c5-127">Remarks</span></span>

<span data-ttu-id="2e4c5-p103">A maioria dos usuários só terá um único recurso Drive. Grupos e alguns usuários podem ter várias unidades disponíveis.</span><span class="sxs-lookup"><span data-stu-id="2e4c5-p103">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/List Drives"
}-->
