---
title: Baixar o conteúdo de um recurso do DriveItemVersion
description: Recuperar o conteúdo de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 2afa8aadb250f9c3450727f9e8fc74cbdad1aea2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726351"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="c3142-103">Baixar o conteúdo de um recurso do DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="c3142-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="c3142-104">Recuperar o conteúdo de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c3142-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3142-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3142-105">Permissions</span></span>

<span data-ttu-id="c3142-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3142-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3142-108">Permission type</span></span>      | <span data-ttu-id="c3142-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3142-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3142-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3142-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3142-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3142-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3142-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3142-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3142-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3142-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3142-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3142-114">Application</span></span> | <span data-ttu-id="c3142-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3142-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c3142-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3142-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="c3142-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3142-117">Response</span></span>

<span data-ttu-id="c3142-118">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3142-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="c3142-p102">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3142-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="c3142-121">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="c3142-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="c3142-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3142-122">Example</span></span>

<span data-ttu-id="c3142-123">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="c3142-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="c3142-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3142-124">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3142-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3142-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3142-126">C#</span><span class="sxs-lookup"><span data-stu-id="c3142-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3142-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3142-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3142-128">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c3142-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c3142-129">Java</span><span class="sxs-lookup"><span data-stu-id="c3142-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c3142-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3142-130">Response</span></span>

<span data-ttu-id="c3142-131">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="c3142-131">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="c3142-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="c3142-132">Remarks</span></span>

<span data-ttu-id="c3142-133">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3142-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="c3142-134">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="c3142-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
