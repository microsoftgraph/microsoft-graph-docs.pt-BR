---
author: JeremyKelley
description: 'Recuperar o conteúdo de uma versão específica de um driveItem. '
ms.date: 09/10/2017
title: Baixar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c7ed8f8100a7910a79569a7e017f37d3d636a26c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956949"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="89aa4-103">Baixar o conteúdo de um recurso de DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="89aa4-103">Download contents of a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89aa4-104">Recuperar o conteúdo de uma versão específica de um [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="89aa4-104">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="89aa4-105">**Observação:** Não há suporte para obter o conteúdo da versão atual.</span><span class="sxs-lookup"><span data-stu-id="89aa4-105">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="89aa4-106">Em vez disso, use o [ponto de extremidade de conteúdo driveItem](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="89aa4-106">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89aa4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="89aa4-107">Permissions</span></span>

<span data-ttu-id="89aa4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89aa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89aa4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89aa4-110">Permission type</span></span>      | <span data-ttu-id="89aa4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89aa4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89aa4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89aa4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="89aa4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89aa4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="89aa4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89aa4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89aa4-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89aa4-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="89aa4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89aa4-116">Application</span></span> | <span data-ttu-id="89aa4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89aa4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="89aa4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89aa4-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="89aa4-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="89aa4-119">Response</span></span>

<span data-ttu-id="89aa4-120">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="89aa4-120">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="89aa4-p103">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="89aa4-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="89aa4-123">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="89aa4-123">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="89aa4-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89aa4-124">Example</span></span>

<span data-ttu-id="89aa4-125">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="89aa4-125">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="89aa4-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89aa4-126">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="89aa4-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="89aa4-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89aa4-128">C#</span><span class="sxs-lookup"><span data-stu-id="89aa4-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89aa4-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="89aa4-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89aa4-130">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="89aa4-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89aa4-131">Java</span><span class="sxs-lookup"><span data-stu-id="89aa4-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89aa4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="89aa4-132">Response</span></span>

<span data-ttu-id="89aa4-133">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="89aa4-133">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="89aa4-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="89aa4-134">Remarks</span></span>

<span data-ttu-id="89aa4-135">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="89aa4-135">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="89aa4-136">Quando o aplicativo recupera a lista de versões disponíveis para um arquivo, um recurso [driveItemVersion](../resources/driveitemversion.md) é retornado que fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="89aa4-136">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->
