# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="bbf9b-101">Listar versões de um item de lista</span><span class="sxs-lookup"><span data-stu-id="bbf9b-101">Listing versions of a ListItem (preview)</span></span>

<span data-ttu-id="bbf9b-102">O SharePoint pode ser configurado para manter o histórico de itens de lista.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-102">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="bbf9b-103">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-103">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbf9b-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbf9b-104">Permissions</span></span>

<span data-ttu-id="bbf9b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bbf9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="bbf9b-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf9b-107">Permission type</span></span>             | <span data-ttu-id="bbf9b-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bbf9b-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbf9b-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf9b-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="bbf9b-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf9b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf9b-112">n/d</span><span class="sxs-lookup"><span data-stu-id="bbf9b-112">n/a</span></span>                                         |
| <span data-ttu-id="bbf9b-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf9b-113">Application</span></span>                            | <span data-ttu-id="bbf9b-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf9b-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="bbf9b-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf9b-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="bbf9b-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf9b-116">Response</span></span>

<span data-ttu-id="bbf9b-117">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf9b-117">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="bbf9b-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf9b-118">Example</span></span>

<span data-ttu-id="bbf9b-119">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="bbf9b-119">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="bbf9b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf9b-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="bbf9b-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf9b-121">Response</span></span>

<span data-ttu-id="bbf9b-122">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="bbf9b-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

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
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
