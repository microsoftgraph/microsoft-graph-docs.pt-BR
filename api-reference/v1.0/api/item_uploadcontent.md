# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="6cd11-101">Carregue ou substitua o conteúdo de um driveItem</span><span class="sxs-lookup"><span data-stu-id="6cd11-101">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="6cd11-p101">A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.</span><span class="sxs-lookup"><span data-stu-id="6cd11-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="6cd11-104">Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="6cd11-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cd11-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6cd11-105">Permissions</span></span>
<span data-ttu-id="6cd11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6cd11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6cd11-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cd11-108">Permission type</span></span>      | <span data-ttu-id="6cd11-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6cd11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cd11-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cd11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6cd11-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd11-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6cd11-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cd11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cd11-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd11-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6cd11-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cd11-114">Application</span></span> | <span data-ttu-id="6cd11-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd11-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cd11-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cd11-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <a name="request-body"></a><span data-ttu-id="6cd11-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cd11-117">Request body</span></span>
<span data-ttu-id="6cd11-118">O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="6cd11-118">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="6cd11-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd11-119">Response</span></span>

<span data-ttu-id="6cd11-120">Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="6cd11-120">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example"></a><span data-ttu-id="6cd11-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cd11-121">Example</span></span>
<span data-ttu-id="6cd11-122">Este exemplo carrega um arquivo pelo caminho do OneDrive do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="6cd11-122">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

##### <a name="response"></a><span data-ttu-id="6cd11-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cd11-123">Response</span></span>

<span data-ttu-id="6cd11-124">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="6cd11-124">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "myfile.jpg",
  "size": 10191,
  "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upload item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
