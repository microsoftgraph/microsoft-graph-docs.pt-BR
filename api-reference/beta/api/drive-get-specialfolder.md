---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter Pastas Especiais
ms.openlocfilehash: 8b8b1186682421a5ab564272fd473cb72819202d
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748497"
---
# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="0e8f6-102">Obtenha uma pasta especial por nome</span><span class="sxs-lookup"><span data-stu-id="0e8f6-102">Get a special folder by name</span></span>

> <span data-ttu-id="0e8f6-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e8f6-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e8f6-105">Use a coleção especial para acessar uma pasta especial pelo nome.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-105">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="0e8f6-p102">Pastas especiais fornecem aliases simples para acessar pastas conhecidas no OneDrive sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a localizar a pasta.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-p102">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="0e8f6-p103">As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

> <span data-ttu-id="0e8f6-110">**Observação:**  Se tiver permissões somente leitura e solicitar uma pasta especial que não exista, você receberá um erro `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-110">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e8f6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e8f6-111">Permissions</span></span>

<span data-ttu-id="0e8f6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e8f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="0e8f6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e8f6-114">Permission type</span></span>             |                                           <span data-ttu-id="0e8f6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e8f6-115">Permissions (from least to most privileged)</span></span>                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0e8f6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e8f6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e8f6-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8f6-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                            |
| <span data-ttu-id="0e8f6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e8f6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e8f6-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8f6-119">Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
| <span data-ttu-id="0e8f6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e8f6-120">Application</span></span>                            | <span data-ttu-id="0e8f6-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8f6-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                                                         |

## <a name="http-request"></a><span data-ttu-id="0e8f6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e8f6-122">HTTP Request</span></span>

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a><span data-ttu-id="0e8f6-123">Nomes de pasta especial</span><span class="sxs-lookup"><span data-stu-id="0e8f6-123">Special folder names</span></span>

<span data-ttu-id="0e8f6-124">Os nomes de pasta especial a seguir estão disponíveis no OneDrive e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-124">The follow special folder names are available in OneDrive and OneDrive for Business.</span></span>

| <span data-ttu-id="0e8f6-125">Name</span><span class="sxs-lookup"><span data-stu-id="0e8f6-125">Name</span></span>        | <span data-ttu-id="0e8f6-126">Id da pasta</span><span class="sxs-lookup"><span data-stu-id="0e8f6-126">Folder id</span></span>    | <span data-ttu-id="0e8f6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e8f6-127">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="0e8f6-128">Documentos</span><span class="sxs-lookup"><span data-stu-id="0e8f6-128">Documents</span></span>   | `documents`  | <span data-ttu-id="0e8f6-129">A pasta Documentos.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-129">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="0e8f6-130">Fotos</span><span class="sxs-lookup"><span data-stu-id="0e8f6-130">Photos</span></span>      | `photos`     | <span data-ttu-id="0e8f6-131">A pasta Fotos.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-131">The Photos folder.</span></span>                                                       |
| <span data-ttu-id="0e8f6-132">Imagens da Câmera</span><span class="sxs-lookup"><span data-stu-id="0e8f6-132">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="0e8f6-133">A pasta de Backup de Imagens da Câmera.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-133">The Camera Roll Backup folder.</span></span>                                           |
| <span data-ttu-id="0e8f6-134">Raiz de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e8f6-134">App Root</span></span>    | `approot`    | <span data-ttu-id="0e8f6-p105">Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}`</span><span class="sxs-lookup"><span data-stu-id="0e8f6-p105">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="0e8f6-137">Música</span><span class="sxs-lookup"><span data-stu-id="0e8f6-137">Music</span></span>       | `music`      | <span data-ttu-id="0e8f6-138">Pasta Música.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-138">The Music folder.</span></span>                                                        |


### <a name="optional-query-parameters"></a><span data-ttu-id="0e8f6-139">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e8f6-139">Optional query parameters</span></span>

<span data-ttu-id="0e8f6-140">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) `$expand` e `$select` para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-140">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="0e8f6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8f6-141">Response</span></span>

<span data-ttu-id="0e8f6-142">Este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-142">This method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

<span data-ttu-id="0e8f6-143">Você pode usar esse método de lidar com uma pasta especial em linha com chamadas adicionais para propriedades ou relações no driveItem.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-143">You can use this method of addressing a special folder inline with additional calls to properties or relationships on the driveItem.</span></span>

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

## <a name="get-children-of-a-special-folder"></a><span data-ttu-id="0e8f6-144">Obter filhos de uma pasta especial</span><span class="sxs-lookup"><span data-stu-id="0e8f6-144">Get children of a special folder</span></span>

<span data-ttu-id="0e8f6-145">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](/graph/query-parameters) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-145">To request the children of a special folder, you can request the `children` collection or use the [expand](/graph/query-parameters) option to expand the children collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="0e8f6-146">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e8f6-146">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="response"></a><span data-ttu-id="0e8f6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e8f6-147">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="0e8f6-148">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e8f6-148">Remarks</span></span>

> <span data-ttu-id="0e8f6-149">**Observação:** A faceta `specialFolder` de DriveItems indica que o item é uma pasta especial e pode ser acessado pelo conjunto `special`.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-149">**Note:** DriveItems with the `specialFolder` facet indicate the item is a special folder and can be accessed via the `special` collection.</span></span>

<span data-ttu-id="0e8f6-150">Se seu aplicativo tiver permissões somente leitura, a solicitação para obter uma pasta especial ou os filhos de uma pasta especial poderá falhar com um erro `404 Not Found` ou `403 Forbidden`, se a pasta especial ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="0e8f6-150">If your app has read-only permissions, the request to get a special folder or the children of a special folder may fail with a `404 Not Found` or a `403 Forbidden` error if the special folder does not already exist.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
