# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="31c37-101">Listar itens compartilhados com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="31c37-101">List items shared with the signed-in user</span></span>

<span data-ttu-id="31c37-102">Recupere uma coleção de recursos [DriveItem](../resources/driveitem.md) que foram compartilhados com o proprietário de [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="31c37-102">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="31c37-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="31c37-103">Permissions</span></span>
<span data-ttu-id="31c37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="31c37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="31c37-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31c37-106">Permission type</span></span>      | <span data-ttu-id="31c37-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31c37-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31c37-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31c37-108">Delegated (work or school account)</span></span> | <span data-ttu-id="31c37-109">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c37-109">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="31c37-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31c37-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31c37-111">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c37-111">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="31c37-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31c37-112">Application</span></span> | <span data-ttu-id="31c37-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31c37-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="31c37-114">Além disso, sem um dos escopos **All**, os itens compartilhados retornados dessa API não ficarão acessíveis.</span><span class="sxs-lookup"><span data-stu-id="31c37-114">Note: while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite scopes, some properties may be missing. Additionally, without one of the  **All** scopes, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="31c37-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31c37-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/sharedWithMe
```

## <a name="request-body"></a><span data-ttu-id="31c37-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31c37-116">Request body</span></span>
<span data-ttu-id="31c37-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31c37-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="31c37-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31c37-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-sharedwithme", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="31c37-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="31c37-119">Response</span></span>

<span data-ttu-id="31c37-p102">Isso retorna uma coleção de recursos [DriveItem](../resources/driveitem.md) que contêm DriveItem recursos compartilhados com o proprietário da unidade. Neste exemplo, como a unidade é a do usuário padrão, isso retorna itens compartilhados com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="31c37-p102">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
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
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="31c37-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="31c37-122">Remarks</span></span>

<span data-ttu-id="31c37-p103">DriveItems retornados da ação **sharedWithMe** sempre incluirão a faceta [**remoteItem**](../resources/remoteitem.md), que indica que são itens de uma unidade diferente. Para acessar o recurso compartilhado DriveItem, você precisará fazer uma solicitação usando as informações fornecidas em **remoteItem** no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="31c37-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
