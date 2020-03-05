---
author: JeremyKelley
description: Recupere os metadados de um DriveItem em um Drive por ID ou por caminho do sistema de arquivos.
ms.date: 09/10/2017
title: obter um arquivo ou uma pasta
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e496682671eea4a7cebfca72789d5d85fe9f3366
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432576"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="61cc4-103">Obter um recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="61cc4-103">Get a DriveItem resource</span></span>

<span data-ttu-id="61cc4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61cc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61cc4-105">Recupere os metadados de um [DriveItem](../resources/driveitem.md) em um [Drive](../resources/drive.md) por ID ou caminho do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="61cc4-105">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="61cc4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="61cc4-106">Permissions</span></span>

<span data-ttu-id="61cc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61cc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61cc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61cc4-109">Permission type</span></span>      | <span data-ttu-id="61cc4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61cc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61cc4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61cc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="61cc4-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span> </br><span data-ttu-id="61cc4-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-113">Group.Read.All, Group.ReadWrite.All</span></span> </br><span data-ttu-id="61cc4-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="61cc4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61cc4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61cc4-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="61cc4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61cc4-117">Application</span></span> | <span data-ttu-id="61cc4-118">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-118">Files.Read.All, Files.ReadWrite.All</span></span> </br><span data-ttu-id="61cc4-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-119">Group.Read.All, Group.ReadWrite.All</span></span> </br><span data-ttu-id="61cc4-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cc4-120">Sites.Read.All, Sites.ReadWrite.All</span></span> |

> <span data-ttu-id="61cc4-121">Observação: o `/teams` ponto de extremidade requer o uso de permissões Group. Read. All ou Group. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="61cc4-121">Note: The `/teams` endpoint requires the use of Group.Read.All or Group.ReadWrite.All permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="61cc4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61cc4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /teams/{teamId}/channels/{channelId}/filesFolder
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61cc4-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61cc4-123">Optional query parameters</span></span>

<span data-ttu-id="61cc4-124">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc4-124">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="61cc4-125">É possível usar o parâmetro de cadeia de caracteres de consulta [`$expand` ](/graph/query-parameters) para incluir os filhos de um item na mesma chamada de recuperação de metadados de um item se item tiver um relacionamento **children**.</span><span class="sxs-lookup"><span data-stu-id="61cc4-125">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<span data-ttu-id="61cc4-126">Você também pode usar o `includeDeletedItems=true` parâmetro de consulta para retornar itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="61cc4-126">You can also use the `includeDeletedItems=true` query parameter to return deleted items.</span></span>
<span data-ttu-id="61cc4-127">Esse parâmetro de consulta só é válido ao direcionar um [driveItem](../resources/driveitem.md) por ID e, caso contrário, será ignorado.</span><span class="sxs-lookup"><span data-stu-id="61cc4-127">This query parameter is only valid when targeting a [driveItem](../resources/driveitem.md) by ID, and otherwise will be ignored.</span></span>
<span data-ttu-id="61cc4-128">No momento, isso só tem suporte no OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="61cc4-128">This is currently only supported on OneDrive Personal.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="61cc4-129">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="61cc4-129">Optional request headers</span></span>

| <span data-ttu-id="61cc4-130">Nome</span><span class="sxs-lookup"><span data-stu-id="61cc4-130">Name</span></span>          | <span data-ttu-id="61cc4-131">Valor</span><span class="sxs-lookup"><span data-stu-id="61cc4-131">Value</span></span>  | <span data-ttu-id="61cc4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61cc4-132">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="61cc4-133">if-none-match</span><span class="sxs-lookup"><span data-stu-id="61cc4-133">if-none-match</span></span> | <span data-ttu-id="61cc4-134">String</span><span class="sxs-lookup"><span data-stu-id="61cc4-134">String</span></span> | <span data-ttu-id="61cc4-135">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida corresponder à marca atual do arquivo, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="61cc4-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="61cc4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cc4-136">Response</span></span>

<span data-ttu-id="61cc4-137">Se bem sucedido, este método retorna o código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc4-137">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61cc4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61cc4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="61cc4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61cc4-139">Request</span></span>

<span data-ttu-id="61cc4-140">Eis um exemplo de solicitação para a pasta raiz do OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="61cc4-140">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

# <a name="http"></a>[<span data-ttu-id="61cc4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="61cc4-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```msgraph-interactive
GET /me/drive/root
```
# <a name="c"></a>[<span data-ttu-id="61cc4-142">C#</span><span class="sxs-lookup"><span data-stu-id="61cc4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-metadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61cc4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61cc4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-metadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61cc4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61cc4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-metadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

## <a name="response"></a><span data-ttu-id="61cc4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="61cc4-145">Response</span></span>

<span data-ttu-id="61cc4-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61cc4-146">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="61cc4-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="61cc4-147">Remarks</span></span>

<span data-ttu-id="61cc4-148">Confira mais informações sobre como os erros são retornados em [Respostas de Erros][error-response].</span><span class="sxs-lookup"><span data-stu-id="61cc4-148">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
}
-->
