---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter pastas especiais
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 019852314e905e16d157637e70f3fa2231564c45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861590"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="c0d96-102">Obtenha uma pasta especial por nome</span><span class="sxs-lookup"><span data-stu-id="c0d96-102">Get a special folder by name</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0d96-103">Use a coleção especial para acessar uma pasta especial pelo nome.</span><span class="sxs-lookup"><span data-stu-id="c0d96-103">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="c0d96-p101">Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.</span><span class="sxs-lookup"><span data-stu-id="c0d96-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="c0d96-p102">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="c0d96-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="c0d96-108">**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="c0d96-108">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0d96-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0d96-109">Permissions</span></span>

<span data-ttu-id="c0d96-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0d96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c0d96-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0d96-112">Permission type</span></span>             |                                           <span data-ttu-id="c0d96-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0d96-113">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c0d96-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0d96-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0d96-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d96-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="c0d96-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0d96-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0d96-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d96-117">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="c0d96-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0d96-118">Application</span></span>                            | <span data-ttu-id="c0d96-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0d96-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="c0d96-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d96-120">HTTP Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c0d96-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d96-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0d96-122">C#</span><span class="sxs-lookup"><span data-stu-id="c0d96-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-folder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d96-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d96-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-folder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0d96-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c0d96-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-folder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0d96-125">Java</span><span class="sxs-lookup"><span data-stu-id="c0d96-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-folder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="special-folder-names"></a><span data-ttu-id="c0d96-126">Nomes de pasta especial</span><span class="sxs-lookup"><span data-stu-id="c0d96-126">Special folder names</span></span>

<span data-ttu-id="c0d96-127">Os nomes de pasta especial a seguir estão disponíveis no OneDrive e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c0d96-127">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="c0d96-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c0d96-128">Name</span></span>        | <span data-ttu-id="c0d96-129">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="c0d96-129">Folder id</span></span>    | <span data-ttu-id="c0d96-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0d96-130">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="c0d96-131">Documentos</span><span class="sxs-lookup"><span data-stu-id="c0d96-131">Documents</span></span>   | `documents`  | <span data-ttu-id="c0d96-132">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="c0d96-132">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="c0d96-133">Fotos</span><span class="sxs-lookup"><span data-stu-id="c0d96-133">Photos</span></span>      | `photos`     | <span data-ttu-id="c0d96-134">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="c0d96-134">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="c0d96-135">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="c0d96-135">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="c0d96-136">A pasta de Backup de Imagens da Câmera.</span><span class="sxs-lookup"><span data-stu-id="c0d96-136">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="c0d96-137">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0d96-137">App Root</span></span>    | `approot`    | <span data-ttu-id="c0d96-p104">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="c0d96-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="c0d96-140">Música</span><span class="sxs-lookup"><span data-stu-id="c0d96-140">Music</span></span>       | `music`      | <span data-ttu-id="c0d96-141">Pasta Música.</span><span class="sxs-lookup"><span data-stu-id="c0d96-141">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="c0d96-142">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c0d96-142">Optional query parameters</span></span>

<span data-ttu-id="c0d96-143">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c0d96-143">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="c0d96-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d96-144">Response</span></span>

<span data-ttu-id="c0d96-145">Este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0d96-145">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="c0d96-146">Você pode usar esse método de lidar com uma pasta especial em linha com chamadas adicionais para propriedades ou relações no driveItem.</span><span class="sxs-lookup"><span data-stu-id="c0d96-146">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="c0d96-147">Obter filhos de uma pasta especial</span><span class="sxs-lookup"><span data-stu-id="c0d96-147">Get children of a special folder</span></span>

<span data-ttu-id="c0d96-148">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](/graph/query-parameters) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="c0d96-148">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="c0d96-149">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d96-149">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c0d96-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0d96-150">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0d96-151">C#</span><span class="sxs-lookup"><span data-stu-id="c0d96-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-special-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0d96-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0d96-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-special-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0d96-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c0d96-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-special-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0d96-154">Java</span><span class="sxs-lookup"><span data-stu-id="c0d96-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-special-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0d96-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0d96-155">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="c0d96-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0d96-156">Remarks</span></span>

> <span data-ttu-id="c0d96-157">**Observação:** A faceta `specialFolder` de DriveItems indica que o item é uma pasta especial e pode ser acessado pelo conjunto `special`.</span><span class="sxs-lookup"><span data-stu-id="c0d96-157">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="c0d96-158">Se seu aplicativo tiver permissões somente leitura, a solicitação para obter uma pasta especial ou os filhos de uma pasta especial poderá falhar com um erro `404 Not Found` ou `403 Forbidden`, se a pasta especial ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="c0d96-158">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
  ]
}
-->
