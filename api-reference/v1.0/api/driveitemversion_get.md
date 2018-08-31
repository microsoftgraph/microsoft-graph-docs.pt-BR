# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="0e197-101">Obter um recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="0e197-101">Get a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="0e197-102">Recuperar os metadados de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0e197-102">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e197-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e197-103">Permissions</span></span>

<span data-ttu-id="0e197-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e197-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e197-106">Permission type</span></span>      | <span data-ttu-id="0e197-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e197-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e197-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e197-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0e197-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e197-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e197-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e197-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e197-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e197-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e197-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e197-112">Application</span></span> | <span data-ttu-id="0e197-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e197-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="0e197-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e197-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="0e197-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e197-115">Response</span></span>

<span data-ttu-id="0e197-116">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [DriveItemVersion](../resources/driveitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e197-116">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="0e197-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e197-117">Example</span></span>

<span data-ttu-id="0e197-118">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="0e197-118">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="0e197-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e197-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="0e197-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e197-120">Response</span></span>

<span data-ttu-id="0e197-121">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="0e197-121">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="0e197-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e197-122">Remarks</span></span>

<span data-ttu-id="0e197-123">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="0e197-123">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="0e197-124">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveItemVersion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="0e197-124">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
