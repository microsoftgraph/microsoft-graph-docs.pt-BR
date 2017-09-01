# <a name="get-drive"></a><span data-ttu-id="ee46f-101">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="ee46f-101">Get Drive</span></span>

<span data-ttu-id="ee46f-p101">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md). Uma Unidade é o contêiner de nível superior para um sistema de arquivos. A API do Graph permite o acesso ao recurso de Unidade do OneDrive ou do OneDrive for Business de um usuário ou a bibliotecas de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ee46f-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee46f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee46f-105">Permissions</span></span>

<span data-ttu-id="ee46f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee46f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee46f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee46f-108">Permission type</span></span>      | <span data-ttu-id="ee46f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee46f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee46f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee46f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee46f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee46f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee46f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee46f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee46f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee46f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee46f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee46f-114">Application</span></span> | <span data-ttu-id="ee46f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee46f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-a-users-onedrive"></a><span data-ttu-id="ee46f-116">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="ee46f-116">Get a user's OneDrive</span></span>

<span data-ttu-id="ee46f-117">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso [User](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ee46f-117">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="ee46f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee46f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="ee46f-119">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="ee46f-119">Get the document library associated with a group</span></span>

<span data-ttu-id="ee46f-120">Para acessar uma biblioteca de documentos padrão [de um Grupo](../resources/group.md), o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="ee46f-120">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="ee46f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee46f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="ee46f-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee46f-122">Optional query parameters</span></span>

<span data-ttu-id="ee46f-123">Este método oferece suporte aos [parâmetros de consulta OData](../../../concepts/query_parameters.md) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46f-123">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="ee46f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee46f-124">Request body</span></span>

<span data-ttu-id="ee46f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee46f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee46f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee46f-126">Response</span></span>

<span data-ttu-id="ee46f-127">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46f-127">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee46f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee46f-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee46f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee46f-129">Request</span></span>

<span data-ttu-id="ee46f-130">Aqui está um exemplo da solicitação para obter o OneDrive ou o OneDrive for Business do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ee46f-130">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="ee46f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee46f-131">Response</span></span>

<span data-ttu-id="ee46f-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46f-132">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
