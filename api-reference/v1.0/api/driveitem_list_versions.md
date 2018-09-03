# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="ffe44-101">Listando versões de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="ffe44-101">Listing versions of a DriveItem (preview)</span></span>

<span data-ttu-id="ffe44-102">O OneDrive e o SharePoint podem ser configurados para manter o histórico de arquivos.</span><span class="sxs-lookup"><span data-stu-id="ffe44-102">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="ffe44-103">Dependendo do serviço e da configuração, uma nova versão pode ser criada para cada edição, sempre que o arquivo for salvo, manualmente ou nunca.</span><span class="sxs-lookup"><span data-stu-id="ffe44-103">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="ffe44-104">Versões anteriores de um documento podem ser retidas por um determinado período dependendo das configurações de administração, que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="ffe44-104">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffe44-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ffe44-105">Permissions</span></span>

<span data-ttu-id="ffe44-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ffe44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffe44-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffe44-108">Permission type</span></span>      | <span data-ttu-id="ffe44-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ffe44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffe44-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffe44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ffe44-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe44-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffe44-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffe44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffe44-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe44-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffe44-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffe44-114">Application</span></span> | <span data-ttu-id="ffe44-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe44-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ffe44-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffe44-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="ffe44-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffe44-117">Response</span></span>

<span data-ttu-id="ffe44-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffe44-118">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="ffe44-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffe44-119">Example</span></span>

<span data-ttu-id="ffe44-120">Este exemplo recupera as versões de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="ffe44-120">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ffe44-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffe44-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="ffe44-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffe44-122">Response</span></span>

<span data-ttu-id="ffe44-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="ffe44-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="ffe44-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="ffe44-124">Remarks</span></span>

<span data-ttu-id="ffe44-125">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="ffe44-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ffe44-126">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveItemVersion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="ffe44-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
