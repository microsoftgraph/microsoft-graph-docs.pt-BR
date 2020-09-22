---
author: JeremyKelley
description: Recupere as propriedades e as relações de um recurso Drive.
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 579a0e59c3227056ade1587f83cbe69911ecd9fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982273"
---
# <a name="get-drive"></a><span data-ttu-id="27501-103">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="27501-103">Get Drive</span></span>

<span data-ttu-id="27501-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27501-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27501-105">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="27501-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="27501-106">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27501-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="27501-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27501-107">Permissions</span></span>

<span data-ttu-id="27501-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27501-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27501-110">Permission type</span></span>      | <span data-ttu-id="27501-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27501-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27501-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27501-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27501-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27501-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="27501-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27501-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27501-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27501-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="27501-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27501-116">Application</span></span> | <span data-ttu-id="27501-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27501-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="27501-118">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="27501-118">Get current user's OneDrive</span></span>

<span data-ttu-id="27501-119">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="27501-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="27501-120">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="27501-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="27501-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="27501-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="27501-123">C#</span><span class="sxs-lookup"><span data-stu-id="27501-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27501-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27501-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27501-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27501-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="27501-126">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="27501-126">Get a user's OneDrive</span></span>

<span data-ttu-id="27501-127">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="27501-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="27501-128">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="27501-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="27501-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-129">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="27501-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="27501-131">C#</span><span class="sxs-lookup"><span data-stu-id="27501-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27501-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27501-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27501-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27501-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="27501-134">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="27501-134">Path parameters</span></span>

| <span data-ttu-id="27501-135">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="27501-135">Parameter name</span></span> | <span data-ttu-id="27501-136">Valor</span><span class="sxs-lookup"><span data-stu-id="27501-136">Value</span></span>  | <span data-ttu-id="27501-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="27501-137">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="27501-138">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="27501-138">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="27501-139">string</span><span class="sxs-lookup"><span data-stu-id="27501-139">string</span></span> | <span data-ttu-id="27501-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27501-140">Required.</span></span> <span data-ttu-id="27501-141">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="27501-141">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="27501-142">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="27501-142">Get the document library associated with a group</span></span>

<span data-ttu-id="27501-143">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="27501-143">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="27501-144">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-144">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="27501-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="27501-146">C#</span><span class="sxs-lookup"><span data-stu-id="27501-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27501-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27501-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27501-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27501-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="27501-149">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="27501-149">Path parameters</span></span>

| <span data-ttu-id="27501-150">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="27501-150">Parameter name</span></span> | <span data-ttu-id="27501-151">Valor</span><span class="sxs-lookup"><span data-stu-id="27501-151">Value</span></span>  | <span data-ttu-id="27501-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="27501-152">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="27501-153">_groupId_</span><span class="sxs-lookup"><span data-stu-id="27501-153">_groupId_</span></span>      | <span data-ttu-id="27501-154">string</span><span class="sxs-lookup"><span data-stu-id="27501-154">string</span></span> | <span data-ttu-id="27501-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27501-155">Required.</span></span> <span data-ttu-id="27501-156">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="27501-156">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="27501-157">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="27501-157">Get the document library for a site</span></span>

<span data-ttu-id="27501-158">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="27501-158">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="27501-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-159">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="27501-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-160">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="27501-161">C#</span><span class="sxs-lookup"><span data-stu-id="27501-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27501-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27501-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27501-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27501-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="27501-164">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="27501-164">Path parameters</span></span>

| <span data-ttu-id="27501-165">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="27501-165">Parameter name</span></span> | <span data-ttu-id="27501-166">Valor</span><span class="sxs-lookup"><span data-stu-id="27501-166">Value</span></span>  | <span data-ttu-id="27501-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="27501-167">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="27501-168">_siteId_</span><span class="sxs-lookup"><span data-stu-id="27501-168">_siteId_</span></span>       | <span data-ttu-id="27501-169">string</span><span class="sxs-lookup"><span data-stu-id="27501-169">string</span></span> | <span data-ttu-id="27501-170">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27501-170">Required.</span></span> <span data-ttu-id="27501-171">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="27501-171">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="27501-172">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="27501-172">Get a drive by ID</span></span>

<span data-ttu-id="27501-173">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="27501-173">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="27501-174">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-174">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="27501-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="27501-175">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{driveId}
```
# <a name="c"></a>[<span data-ttu-id="27501-176">C#</span><span class="sxs-lookup"><span data-stu-id="27501-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27501-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27501-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27501-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27501-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="27501-179">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="27501-179">Path parameters</span></span>

| <span data-ttu-id="27501-180">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="27501-180">Parameter name</span></span> | <span data-ttu-id="27501-181">Valor</span><span class="sxs-lookup"><span data-stu-id="27501-181">Value</span></span>  | <span data-ttu-id="27501-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="27501-182">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="27501-183">_driveId_</span><span class="sxs-lookup"><span data-stu-id="27501-183">_driveId_</span></span>      | <span data-ttu-id="27501-184">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27501-184">string</span></span> | <span data-ttu-id="27501-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="27501-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="27501-187">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27501-187">Optional query parameters</span></span>

<span data-ttu-id="27501-188">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27501-188">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="27501-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="27501-189">Response</span></span>

<span data-ttu-id="27501-190">Cada um desses métodos retorna um [Recurso de Unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27501-190">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="27501-191">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="27501-191">Error response codes</span></span>

<span data-ttu-id="27501-192">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="27501-192">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Microsoft 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->


