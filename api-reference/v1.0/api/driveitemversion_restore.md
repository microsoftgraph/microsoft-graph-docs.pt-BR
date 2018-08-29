# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="ba3c6-101">Restaurar uma versão anterior de um DriveItem</span><span class="sxs-lookup"><span data-stu-id="ba3c6-101">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="ba3c6-102">Restaura uma versão anterior de um DriveItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="ba3c6-102">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="ba3c6-103">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ba3c6-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba3c6-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba3c6-104">Permissions</span></span>

<span data-ttu-id="ba3c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba3c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba3c6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba3c6-107">Permission type</span></span>      | <span data-ttu-id="ba3c6-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba3c6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba3c6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba3c6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ba3c6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3c6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba3c6-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba3c6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba3c6-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3c6-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba3c6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba3c6-113">Application</span></span> | <span data-ttu-id="ba3c6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba3c6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba3c6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba3c6-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="ba3c6-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba3c6-116">Request body</span></span>

<span data-ttu-id="ba3c6-117">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba3c6-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="ba3c6-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba3c6-118">Example</span></span>

<span data-ttu-id="ba3c6-119">Este exemplo restaura uma versão de um arquivo identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="ba3c6-119">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="ba3c6-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba3c6-120">Response</span></span>

<span data-ttu-id="ba3c6-121">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba3c6-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
