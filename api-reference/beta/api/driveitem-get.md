---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a238e1dd459ee04d5c6c7c3453edaac2d569ed84
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589295"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="79e55-102">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="79e55-102">Get a DriveItem resource</span></span>

<span data-ttu-id="79e55-103">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="79e55-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="79e55-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="79e55-104">Permissions</span></span>

<span data-ttu-id="79e55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79e55-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79e55-107">Permission type</span></span>      | <span data-ttu-id="79e55-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="79e55-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79e55-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79e55-109">Delegated (work or school account)</span></span> | <span data-ttu-id="79e55-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79e55-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="79e55-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79e55-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79e55-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79e55-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="79e55-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79e55-113">Application</span></span> | <span data-ttu-id="79e55-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79e55-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79e55-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79e55-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79e55-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="79e55-116">Optional query parameters</span></span>

<span data-ttu-id="79e55-117">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="79e55-117">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="79e55-118">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="79e55-118">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="79e55-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="79e55-119">Optional request headers</span></span>

| <span data-ttu-id="79e55-120">Nome</span><span class="sxs-lookup"><span data-stu-id="79e55-120">Name</span></span>          | <span data-ttu-id="79e55-121">Valor</span><span class="sxs-lookup"><span data-stu-id="79e55-121">Value</span></span>  | <span data-ttu-id="79e55-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="79e55-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="79e55-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="79e55-123">if-none-match</span></span> | <span data-ttu-id="79e55-124">String</span><span class="sxs-lookup"><span data-stu-id="79e55-124">String</span></span> | <span data-ttu-id="79e55-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="79e55-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="79e55-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="79e55-126">Response</span></span>

<span data-ttu-id="79e55-127">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79e55-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79e55-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79e55-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="79e55-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79e55-129">Request</span></span>

<span data-ttu-id="79e55-130">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="79e55-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="79e55-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="79e55-131">Response</span></span>

<span data-ttu-id="79e55-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79e55-132">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="79e55-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="79e55-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="79e55-134">C#</span><span class="sxs-lookup"><span data-stu-id="79e55-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-metadata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79e55-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="79e55-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-metadata-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="79e55-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="79e55-136">Remarks</span></span>

<span data-ttu-id="79e55-137">Confira mais informações sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="79e55-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
