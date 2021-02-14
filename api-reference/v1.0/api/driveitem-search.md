---
author: JeremyKelley
ms.date: 07/07/2020
title: Pesquisar arquivos
localization_priority: Priority
ms.prod: sharepoint
description: Pesquise a hierarquia de itens para itens que corresponda a uma consulta.
doc_type: apiPageType
ms.openlocfilehash: 8cf0095d504f88fbce75aa65c7d733ccf04392d0
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240206"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="58055-103">Pesquisar um DriveItem em uma unidade</span><span class="sxs-lookup"><span data-stu-id="58055-103">Search for a DriveItems within a drive</span></span>

<span data-ttu-id="58055-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58055-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58055-105">Pesquise a hierarquia de itens para itens que correspondam a uma consulta.</span><span class="sxs-lookup"><span data-stu-id="58055-105">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="58055-106">Você pode pesquisar em uma hierarquia de pastas, uma unidade inteira ou arquivos compartilhados com o usuário atual.</span><span class="sxs-lookup"><span data-stu-id="58055-106">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="58055-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="58055-107">Permissions</span></span>

<span data-ttu-id="58055-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58055-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58055-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58055-110">Permission type</span></span>      | <span data-ttu-id="58055-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58055-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58055-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58055-112">Delegated (work or school account)</span></span> | <span data-ttu-id="58055-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58055-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="58055-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58055-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58055-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58055-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="58055-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58055-116">Application</span></span> | <span data-ttu-id="58055-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58055-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58055-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58055-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58055-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58055-119">Optional query parameters</span></span>

<span data-ttu-id="58055-120">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58055-120">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="58055-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="58055-121">Function parameters</span></span>

| <span data-ttu-id="58055-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58055-122">Parameter</span></span> | <span data-ttu-id="58055-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="58055-123">Type</span></span>  | <span data-ttu-id="58055-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="58055-124">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="58055-125">q</span><span class="sxs-lookup"><span data-stu-id="58055-125">q</span></span>  | <span data-ttu-id="58055-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58055-126">string</span></span> | <span data-ttu-id="58055-p103">O texto de consulta usado para pesquisar itens. Os valores podem ser correspondidos em vários campos, incluindo nome do arquivo, metadados e conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="58055-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="58055-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58055-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="58055-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58055-130">Request</span></span>

<span data-ttu-id="58055-131">O exemplo a seguir procura uma correspondência para "Projeto da Contoso" entre vários campos nos itens da unidade do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="58055-131">The following example searches for a match for "Contoso Project" across several fields in the signed-in user's drive items.</span></span>


# <a name="http"></a>[<span data-ttu-id="58055-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="58055-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/root/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="58055-133">C#</span><span class="sxs-lookup"><span data-stu-id="58055-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58055-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58055-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58055-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58055-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58055-136">Java</span><span class="sxs-lookup"><span data-stu-id="58055-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58055-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="58055-137">Response</span></span>

<span data-ttu-id="58055-p104">Este método retorna um objeto que contém uma coleção de [DriveItems](../resources/driveitem.md) que correspondem aos critérios de pesquisa. Se não forem encontrados itens, uma coleção vazia será retornada.</span><span class="sxs-lookup"><span data-stu-id="58055-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="58055-p105">Se houver muitas correspondências, a resposta será paginada e uma propriedade **\@odata.nextLink** incluirá uma URL para a próxima página de resultados. Você pode usar o `$top` parâmetro de consulta para especificar o número de itens na página.</span><span class="sxs-lookup"><span data-stu-id="58055-p105">If there are too many matches the response will be paged and an **\@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

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

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="58055-142">Pesquisando itens que um usuário pode acessar</span><span class="sxs-lookup"><span data-stu-id="58055-142">Searching for items a user can access</span></span>

<span data-ttu-id="58055-p106">Além de procurar itens em uma unidade, seu aplicativo pode pesquisar amplamente para incluir itens compartilhados com o usuário atual. Para ampliar o escopo da pesquisa, use o método **search** no recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="58055-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="58055-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58055-145">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="58055-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="58055-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "item_search_all", "tags": "service.graph" }-->

```msgraph-interactive
GET /me/drive/search(q='Contoso Project')
```
# <a name="c"></a>[<span data-ttu-id="58055-147">C#</span><span class="sxs-lookup"><span data-stu-id="58055-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-search-all-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58055-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58055-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-search-all-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58055-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58055-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-search-all-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58055-150">Java</span><span class="sxs-lookup"><span data-stu-id="58055-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-search-all-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58055-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="58055-151">Response</span></span>

<span data-ttu-id="58055-p107">As respostas ao pesquisar por meio do recurso **drive** podem incluir itens fora da unidade (itens compartilhados com o usuário atual). Estes itens incluirão a faceta [**remoteItem**](../resources/remoteitem.md) para indicar que estão armazenados fora da unidade de destino.</span><span class="sxs-lookup"><span data-stu-id="58055-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

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

## <a name="error-responses"></a><span data-ttu-id="58055-154">Respostas de erros</span><span class="sxs-lookup"><span data-stu-id="58055-154">Error responses</span></span>

<span data-ttu-id="58055-155">Confira [Respostas de Erros][error-response] para saber mais sobre como os erros retornam.</span><span class="sxs-lookup"><span data-stu-id="58055-155">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

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
  ]
} -->

