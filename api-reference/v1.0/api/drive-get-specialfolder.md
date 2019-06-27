---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter pastas especiais
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b28f7044847bc85b9bde1d2a50ab444b64d70dcb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277095"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="592e9-102">Obtenha uma pasta especial por nome</span><span class="sxs-lookup"><span data-stu-id="592e9-102">Get a special folder by name</span></span>

<span data-ttu-id="592e9-103">Use a coleção especial para acessar uma pasta especial pelo nome.</span><span class="sxs-lookup"><span data-stu-id="592e9-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="592e9-p101">Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.</span><span class="sxs-lookup"><span data-stu-id="592e9-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="592e9-p102">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="592e9-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="592e9-108">**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="592e9-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="592e9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="592e9-109">Permissions</span></span>

<span data-ttu-id="592e9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="592e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="592e9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="592e9-112">Permission type</span></span>             |                                           <span data-ttu-id="592e9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="592e9-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="592e9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="592e9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="592e9-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="592e9-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="592e9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="592e9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="592e9-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="592e9-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="592e9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592e9-118">Application</span></span>                            | <span data-ttu-id="592e9-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="592e9-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="592e9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592e9-120">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="592e9-121">Nomes de pasta especial</span><span class="sxs-lookup"><span data-stu-id="592e9-121">Special folder names</span></span>

<span data-ttu-id="592e9-122">Os nomes de pasta especial a seguir estão disponíveis no OneDrive e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="592e9-122">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="592e9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="592e9-123">Name</span></span>        | <span data-ttu-id="592e9-124">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="592e9-124">Folder id</span></span>    | <span data-ttu-id="592e9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="592e9-125">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="592e9-126">Documentos</span><span class="sxs-lookup"><span data-stu-id="592e9-126">Documents</span></span>   | `documents`  | <span data-ttu-id="592e9-127">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="592e9-127">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="592e9-128">Fotos</span><span class="sxs-lookup"><span data-stu-id="592e9-128">Photos</span></span>      | `photos`     | <span data-ttu-id="592e9-129">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="592e9-129">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="592e9-130">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="592e9-130">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="592e9-131">A pasta de Backup de Imagens da Câmera.</span><span class="sxs-lookup"><span data-stu-id="592e9-131">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="592e9-132">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592e9-132">App Root</span></span>    | `approot`    | <span data-ttu-id="592e9-p104">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="592e9-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="592e9-135">Música</span><span class="sxs-lookup"><span data-stu-id="592e9-135">Music</span></span>       | `music`      | <span data-ttu-id="592e9-136">Pasta Música.</span><span class="sxs-lookup"><span data-stu-id="592e9-136">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="592e9-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="592e9-137">Optional query parameters</span></span>

<span data-ttu-id="592e9-138">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="592e9-138">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="592e9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="592e9-139">Response</span></span>

<span data-ttu-id="592e9-140">Este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="592e9-140">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="592e9-141">Você pode usar esse método de lidar com uma pasta especial em linha com chamadas adicionais para propriedades ou relações no driveItem.</span><span class="sxs-lookup"><span data-stu-id="592e9-141">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="592e9-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="592e9-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="592e9-143">C#</span><span class="sxs-lookup"><span data-stu-id="592e9-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-folder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="592e9-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="592e9-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-folder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="592e9-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="592e9-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-folder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="592e9-146">Obter filhos de uma pasta especial</span><span class="sxs-lookup"><span data-stu-id="592e9-146">Get children of a special folder</span></span>

<span data-ttu-id="592e9-147">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](/graph/query-parameters) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="592e9-147">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="592e9-148">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592e9-148">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```

### <a name="response"></a><span data-ttu-id="592e9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="592e9-149">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="592e9-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="592e9-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="592e9-151">C#</span><span class="sxs-lookup"><span data-stu-id="592e9-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="592e9-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="592e9-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="592e9-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="592e9-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="592e9-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="592e9-154">Remarks</span></span>

> <span data-ttu-id="592e9-155">**Observação:** A faceta `specialFolder` de DriveItems indica que o item é uma pasta especial e pode ser acessado pelo conjunto `special`.</span><span class="sxs-lookup"><span data-stu-id="592e9-155">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="592e9-156">Se seu aplicativo tiver permissões somente leitura, a solicitação para obter uma pasta especial ou os filhos de uma pasta especial poderá falhar com um erro `404 Not Found` ou `403 Forbidden`, se a pasta especial ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="592e9-156">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
