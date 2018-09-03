# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="392bd-101">Restaura uma versão anterior de um ListItem</span><span class="sxs-lookup"><span data-stu-id="392bd-101">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="392bd-102">Restaura uma versão anterior de um ListItem para ser a versão atual.</span><span class="sxs-lookup"><span data-stu-id="392bd-102">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="392bd-103">Isso criará uma nova versão com o conteúdo da versão anterior, mas preservará todas as versões existentes do item.</span><span class="sxs-lookup"><span data-stu-id="392bd-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="392bd-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="392bd-104">Permissions</span></span>

<span data-ttu-id="392bd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="392bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="392bd-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="392bd-107">Permission type</span></span>             |         <span data-ttu-id="392bd-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="392bd-108">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="392bd-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="392bd-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="392bd-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="392bd-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="392bd-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="392bd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="392bd-112">n/d</span><span class="sxs-lookup"><span data-stu-id="392bd-112">n/a</span></span>                                                          |
| <span data-ttu-id="392bd-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="392bd-113">Application</span></span>                            | <span data-ttu-id="392bd-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="392bd-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="392bd-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="392bd-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="392bd-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="392bd-116">Request body</span></span>

<span data-ttu-id="392bd-117">Nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="392bd-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="392bd-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="392bd-118">Example</span></span>

<span data-ttu-id="392bd-119">Este exemplo restaura uma versão de um listItem identificado por `{item-id}` e `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="392bd-119">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="392bd-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="392bd-120">Response</span></span>

<span data-ttu-id="392bd-121">Se tiver êxito, a chamada API retorna um código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="392bd-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
