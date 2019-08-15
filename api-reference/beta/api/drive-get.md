---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso Drive.
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e564303b4d4ac1ad937c10e20c55ee21205947f4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417035"
---
# <a name="get-drive"></a><span data-ttu-id="adb71-103">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="adb71-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb71-104">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="adb71-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="adb71-105">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="adb71-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="adb71-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="adb71-106">Permissions</span></span>

<span data-ttu-id="adb71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adb71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adb71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adb71-109">Permission type</span></span>      | <span data-ttu-id="adb71-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adb71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adb71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adb71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="adb71-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb71-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="adb71-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adb71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adb71-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb71-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="adb71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adb71-115">Application</span></span> | <span data-ttu-id="adb71-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb71-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="adb71-117">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="adb71-117">Get current user's OneDrive</span></span>

<span data-ttu-id="adb71-118">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="adb71-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="adb71-119">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="adb71-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="adb71-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adb71-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adb71-122">C#</span><span class="sxs-lookup"><span data-stu-id="adb71-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adb71-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb71-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adb71-124">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adb71-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="adb71-125">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="adb71-125">Get a user's OneDrive</span></span>

<span data-ttu-id="adb71-126">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="adb71-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="adb71-127">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="adb71-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="adb71-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adb71-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adb71-130">C#</span><span class="sxs-lookup"><span data-stu-id="adb71-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adb71-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb71-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adb71-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adb71-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="adb71-133">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="adb71-133">Path parameters</span></span>

| <span data-ttu-id="adb71-134">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="adb71-134">Parameter name</span></span> | <span data-ttu-id="adb71-135">Valor</span><span class="sxs-lookup"><span data-stu-id="adb71-135">Value</span></span>  | <span data-ttu-id="adb71-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb71-136">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="adb71-137">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="adb71-137">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="adb71-138">string</span><span class="sxs-lookup"><span data-stu-id="adb71-138">string</span></span> | <span data-ttu-id="adb71-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adb71-139">Required.</span></span> <span data-ttu-id="adb71-140">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="adb71-140">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="adb71-141">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="adb71-141">Get the document library associated with a group</span></span>

<span data-ttu-id="adb71-142">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="adb71-142">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="adb71-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-143">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adb71-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adb71-145">C#</span><span class="sxs-lookup"><span data-stu-id="adb71-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adb71-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb71-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adb71-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adb71-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="adb71-148">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="adb71-148">Path parameters</span></span>

| <span data-ttu-id="adb71-149">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="adb71-149">Parameter name</span></span> | <span data-ttu-id="adb71-150">Valor</span><span class="sxs-lookup"><span data-stu-id="adb71-150">Value</span></span>  | <span data-ttu-id="adb71-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb71-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="adb71-152">_groupId_</span><span class="sxs-lookup"><span data-stu-id="adb71-152">_groupId_</span></span>      | <span data-ttu-id="adb71-153">string</span><span class="sxs-lookup"><span data-stu-id="adb71-153">string</span></span> | <span data-ttu-id="adb71-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adb71-154">Required.</span></span> <span data-ttu-id="adb71-155">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="adb71-155">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="adb71-156">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="adb71-156">Get the document library for a site</span></span>

<span data-ttu-id="adb71-157">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="adb71-157">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="adb71-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-158">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adb71-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-159">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adb71-160">C#</span><span class="sxs-lookup"><span data-stu-id="adb71-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adb71-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb71-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adb71-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adb71-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="adb71-163">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="adb71-163">Path parameters</span></span>

| <span data-ttu-id="adb71-164">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="adb71-164">Parameter name</span></span> | <span data-ttu-id="adb71-165">Valor</span><span class="sxs-lookup"><span data-stu-id="adb71-165">Value</span></span>  | <span data-ttu-id="adb71-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb71-166">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="adb71-167">_siteId_</span><span class="sxs-lookup"><span data-stu-id="adb71-167">_siteId_</span></span>       | <span data-ttu-id="adb71-168">string</span><span class="sxs-lookup"><span data-stu-id="adb71-168">string</span></span> | <span data-ttu-id="adb71-169">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adb71-169">Required.</span></span> <span data-ttu-id="adb71-170">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="adb71-170">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="adb71-171">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="adb71-171">Get a drive by ID</span></span>

<span data-ttu-id="adb71-172">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="adb71-172">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="adb71-173">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-173">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="adb71-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="adb71-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="adb71-175">C#</span><span class="sxs-lookup"><span data-stu-id="adb71-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adb71-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adb71-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adb71-177">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="adb71-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="adb71-178">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="adb71-178">Path parameters</span></span>

| <span data-ttu-id="adb71-179">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="adb71-179">Parameter name</span></span> | <span data-ttu-id="adb71-180">Valor</span><span class="sxs-lookup"><span data-stu-id="adb71-180">Value</span></span>  | <span data-ttu-id="adb71-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="adb71-181">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="adb71-182">_driveId_</span><span class="sxs-lookup"><span data-stu-id="adb71-182">_driveId_</span></span>      | <span data-ttu-id="adb71-183">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adb71-183">string</span></span> | <span data-ttu-id="adb71-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="adb71-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="adb71-186">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="adb71-186">Optional query parameters</span></span>

<span data-ttu-id="adb71-187">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="adb71-187">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="adb71-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="adb71-188">Response</span></span>

<span data-ttu-id="adb71-189">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adb71-189">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id",] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="adb71-190">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="adb71-190">Error response codes</span></span>

<span data-ttu-id="adb71-191">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="adb71-191">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->
