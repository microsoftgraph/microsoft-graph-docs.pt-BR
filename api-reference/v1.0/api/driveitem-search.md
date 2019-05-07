---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Pesquisar arquivos
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: c687a79c2dbfbe5ca56710d0bcc4cf4a928dd13d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616299"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="83b5b-102">Pesquisar um DriveItem em uma unidade</span><span class="sxs-lookup"><span data-stu-id="83b5b-102">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="83b5b-103">Pesquise a hierarquia de itens para itens que correspondam a uma consulta.</span><span class="sxs-lookup"><span data-stu-id="83b5b-103">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="83b5b-104">Você pode pesquisar em uma hierarquia de pastas, uma unidade inteira ou arquivos compartilhados com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="83b5b-104">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="83b5b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="83b5b-105">Permissions</span></span>

<span data-ttu-id="83b5b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b5b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83b5b-108">Permission type</span></span>      | <span data-ttu-id="83b5b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83b5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83b5b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83b5b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83b5b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b5b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="83b5b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83b5b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83b5b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b5b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="83b5b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83b5b-114">Application</span></span> | <span data-ttu-id="83b5b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b5b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83b5b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83b5b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="83b5b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83b5b-117">Optional query parameters</span></span>

<span data-ttu-id="83b5b-118">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83b5b-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="83b5b-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="83b5b-119">Function parameters</span></span>

| <span data-ttu-id="83b5b-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="83b5b-120">Parameter</span></span> | <span data-ttu-id="83b5b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="83b5b-121">Type</span></span>  | <span data-ttu-id="83b5b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="83b5b-122">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="83b5b-123">q</span><span class="sxs-lookup"><span data-stu-id="83b5b-123">q</span></span>  | <span data-ttu-id="83b5b-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83b5b-124">string</span></span> | <span data-ttu-id="83b5b-p103">O texto de consulta usado para pesquisar itens. Os valores podem ser correspondidos em vários campos, incluindo nome do arquivo, metadados e conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="83b5b-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="83b5b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83b5b-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="83b5b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83b5b-128">Request</span></span>

<span data-ttu-id="83b5b-129">Aqui está um exemplo da solicitação de que pesquisa o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="83b5b-129">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="83b5b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b5b-130">Response</span></span>

<span data-ttu-id="83b5b-p104">Este método retorna um objeto que contém uma coleção de [DriveItems](../resources/driveitem.md) que correspondem aos critérios de pesquisa. Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="83b5b-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="83b5b-p105">Se houver muitas correspondências, a resposta será paginada, e uma propriedade **@odata.nextLink** conterá uma URL para a próxima página de resultados. Você pode usar o parâmetro de consulta `$top` para especificar o número de itens na página.</span><span class="sxs-lookup"><span data-stu-id="83b5b-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="83b5b-135">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="83b5b-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83b5b-136">C#</span><span class="sxs-lookup"><span data-stu-id="83b5b-136">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/item_search-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83b5b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="83b5b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/item_search-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="83b5b-138">Pesquisando itens que um usuário pode acessar</span><span class="sxs-lookup"><span data-stu-id="83b5b-138">Searching for items a user can access</span></span>

<span data-ttu-id="83b5b-p106">Além de procurar itens em uma unidade, seu aplicativo pode pesquisar amplamente para incluir itens compartilhados com o usuário atual. Para ampliar o escopo da pesquisa, use o método **search** no recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="83b5b-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="83b5b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83b5b-141">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="83b5b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="83b5b-142">Response</span></span>

<span data-ttu-id="83b5b-p107">As respostas ao pesquisar por meio do recurso **drive** podem incluir itens fora da unidade (itens compartilhados com o usuário atual). Estes itens incluirão a faceta [**remoteItem**](../resources/remoteitem.md) para indicar que estão armazenados fora da unidade de destino.</span><span class="sxs-lookup"><span data-stu-id="83b5b-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "parentReference": { "driveId": "s!1020101jlkjl12lx" } }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="83b5b-145">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="83b5b-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="83b5b-146">C#</span><span class="sxs-lookup"><span data-stu-id="83b5b-146">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/item_search_all-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="83b5b-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="83b5b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/item_search_all-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="83b5b-148">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="83b5b-148">Error responses</span></span>

<span data-ttu-id="83b5b-149">Confira [Respostas de erro][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="83b5b-149">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-search.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-search.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-search.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-search.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
