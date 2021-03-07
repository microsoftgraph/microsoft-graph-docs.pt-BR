---
title: Baixar conteúdo de um recurso DriveItemVersion
description: Recuperar o conteúdo de uma versão específica de um DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 739762912030fbaf0a81ef3f2400b5caef8a933a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516791"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="66806-103">Baixar conteúdo de um recurso DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="66806-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="66806-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66806-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66806-105">Recuperar o conteúdo de uma versão específica de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="66806-105">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66806-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66806-106">Permissions</span></span>

<span data-ttu-id="66806-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66806-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66806-109">Permission type</span></span>      | <span data-ttu-id="66806-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66806-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66806-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66806-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66806-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66806-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="66806-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66806-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66806-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66806-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="66806-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66806-115">Application</span></span> | <span data-ttu-id="66806-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66806-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="66806-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66806-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="66806-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="66806-118">Response</span></span>

<span data-ttu-id="66806-119">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="66806-119">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="66806-p102">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="66806-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="66806-122">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="66806-122">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="66806-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66806-123">Example</span></span>

<span data-ttu-id="66806-124">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="66806-124">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="66806-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66806-125">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="66806-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="66806-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="c"></a>[<span data-ttu-id="66806-127">C#</span><span class="sxs-lookup"><span data-stu-id="66806-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66806-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66806-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66806-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66806-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66806-130">Java</span><span class="sxs-lookup"><span data-stu-id="66806-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="66806-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="66806-131">Response</span></span>

<span data-ttu-id="66806-132">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="66806-132">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="66806-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="66806-133">Remarks</span></span>

<span data-ttu-id="66806-134">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="66806-134">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="66806-135">Quando seu aplicativo recupera a lista de versões disponíveis de um arquivo, um recurso [DriveItemVersion](../resources/driveitemversion.md) é retornado e fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="66806-135">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->

