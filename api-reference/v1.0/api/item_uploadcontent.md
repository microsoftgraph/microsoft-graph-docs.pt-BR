<span data-ttu-id="908eb-p101">A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.</span><span class="sxs-lookup"><span data-stu-id="908eb-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

A API de upload simples permite que você forneça o conteúdo de um novo arquivo ou atualize o conteúdo de um arquivo existente em uma única chamada à API. Este método só dá suporte a arquivos com até 4 MB de tamanho.

<span data-ttu-id="908eb-104">Para carregar arquivos grandes, confira [Carregar arquivos grandes com uma sessão de carregamento](item_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="908eb-104">To upload large files see [Upload large files with an upload session](item_createuploadsession.md).</span></span>

## <span data-ttu-id="908eb-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="908eb-105">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="908eb-106">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="908eb-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="908eb-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="908eb-107">Files.ReadWrite</span></span>
* <span data-ttu-id="908eb-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="908eb-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="908eb-109">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="908eb-109">Sites.ReadWrite.All</span></span>


## <span data-ttu-id="908eb-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="908eb-110">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/root:/{parent-path}/{filename}:/content
PUT /me/drive/items/{parent-id}/children/{filename}/content
PUT /groups/{id}/drive/items/{parent-id}/children/{filename}/content
```

## <span data-ttu-id="908eb-111">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="908eb-111">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="908eb-112">O conteúdo do corpo da solicitação deve ser o fluxo binário do arquivo a ser carregado.</span><span class="sxs-lookup"><span data-stu-id="908eb-112">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <span data-ttu-id="908eb-113">Resposta</span><span class="sxs-lookup"><span data-stu-id="908eb-113">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="908eb-114">Se for bem-sucedido, este método retornará um objeto [driveItem](../resources/driveitem.md) no corpo da resposta para o arquivo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="908eb-114">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <span data-ttu-id="908eb-115">Exemplo</span><span class="sxs-lookup"><span data-stu-id="908eb-115">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="908eb-116">Este exemplo carrega um arquivo pelo caminho do OneDrive do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="908eb-116">This example uploads a file by path to the signed-in user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "upload_item"
}-->
```http
PUT /me/drive/root:/{item-path}:/content
Content-type: text/plain

The contents of the file goes here.
```

## <span data-ttu-id="908eb-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="908eb-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="908eb-118">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="908eb-118">Here is an example of the response.</span></span>
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
