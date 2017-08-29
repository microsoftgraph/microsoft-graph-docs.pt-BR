# <a name="list-recent-files"></a><span data-ttu-id="8d857-101">Listar arquivos recentes</span><span class="sxs-lookup"><span data-stu-id="8d857-101">List recent files</span></span>

<span data-ttu-id="8d857-p101">Listar uma coleção de itens que foram usados recentemente pelo usuário conectado. Esta coleção inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades.</span><span class="sxs-lookup"><span data-stu-id="8d857-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d857-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d857-104">Permissions</span></span>
<span data-ttu-id="8d857-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d857-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8d857-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d857-107">Permission type</span></span>      | <span data-ttu-id="8d857-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d857-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d857-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d857-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8d857-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d857-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d857-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d857-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d857-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d857-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d857-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d857-113">Application</span></span> | <span data-ttu-id="8d857-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d857-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d857-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d857-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a><span data-ttu-id="8d857-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d857-116">Request body</span></span>
<span data-ttu-id="8d857-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d857-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="8d857-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d857-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a><span data-ttu-id="8d857-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d857-119">Response</span></span>

<span data-ttu-id="8d857-p103">Isso retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) para itens que o proprietário da unidade acessou recentemente. Itens de fora da unidade do usuário incluirão a faceta [RemoteItem](../resources/remoteitem.md), que fornece informações para acessar o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8d857-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the [RemoteItem](../resources/remoteitem.md) facet, which provides information to access the shared item.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="8d857-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d857-122">Remarks</span></span>

<span data-ttu-id="8d857-p104">Alguns driveItems retornados da ação **recent** incluirão a faceta **remoteItem** que indica que eles são itens de outra unidade. Para acessar o objeto driveItem original, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="8d857-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
