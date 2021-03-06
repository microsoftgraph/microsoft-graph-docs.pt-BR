---
author: JeremyKelley
description: 'Recupere o conteúdo de uma versão específica de um driveItem. '
ms.date: 09/10/2017
title: Baixar uma versão anterior
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c521c3ad4c4776e67747d9f6b09deb5e39fcac82
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515524"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="99584-103">Baixar o conteúdo de um recurso de DriveItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="99584-103">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="99584-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99584-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99584-105">Recupere o conteúdo de uma versão específica de [um driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="99584-105">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="99584-106">**Observação:** Não há suporte para obter o conteúdo da versão atual.</span><span class="sxs-lookup"><span data-stu-id="99584-106">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="99584-107">Em vez disso, use o ponto de extremidade [de conteúdo driveItem](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="99584-107">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99584-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="99584-108">Permissions</span></span>

<span data-ttu-id="99584-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99584-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99584-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99584-111">Permission type</span></span>      | <span data-ttu-id="99584-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99584-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99584-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99584-113">Delegated (work or school account)</span></span> | <span data-ttu-id="99584-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99584-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="99584-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99584-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99584-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99584-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="99584-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99584-117">Application</span></span> | <span data-ttu-id="99584-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99584-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="99584-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99584-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="99584-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="99584-120">Response</span></span>

<span data-ttu-id="99584-121">Retorna uma resposta `302 Found` que redireciona para uma URL de download previamente autenticada para os bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="99584-121">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="99584-p103">Para baixar o conteúdo do arquivo, seu aplicativo precisará seguir o cabeçalho `Location` na resposta. Várias bibliotecas de cliente HTTP seguirão automaticamente o redirecionamento 302 e começarão a baixar imediatamente o arquivo.</span><span class="sxs-lookup"><span data-stu-id="99584-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="99584-124">URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization` para download.</span><span class="sxs-lookup"><span data-stu-id="99584-124">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="99584-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99584-125">Example</span></span>

<span data-ttu-id="99584-126">Este exemplo recupera uma versão de um arquivo na unidade do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="99584-126">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="99584-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99584-127">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="99584-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="99584-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="c"></a>[<span data-ttu-id="99584-129">C#</span><span class="sxs-lookup"><span data-stu-id="99584-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99584-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99584-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99584-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99584-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99584-132">Java</span><span class="sxs-lookup"><span data-stu-id="99584-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99584-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="99584-133">Response</span></span>

<span data-ttu-id="99584-134">Isso retorna um redirecionamento para onde o conteúdo da versão pode ser baixado.</span><span class="sxs-lookup"><span data-stu-id="99584-134">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="99584-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="99584-135">Remarks</span></span>

<span data-ttu-id="99584-136">O OneDrive não preserva os metadados completos de versões anteriores de um arquivo.</span><span class="sxs-lookup"><span data-stu-id="99584-136">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="99584-137">Quando seu aplicativo recupera a lista de versões disponíveis para um arquivo, um [recurso driveItemVersion](../resources/driveitemversion.md) é retornado que fornece as informações disponíveis sobre a versão específica.</span><span class="sxs-lookup"><span data-stu-id="99584-137">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

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


