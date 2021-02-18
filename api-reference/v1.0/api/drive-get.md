---
author: JeremyKelley
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Priority
ms.prod: sharepoint
description: Recupere as propriedades e as relações de um recurso Drive.
doc_type: apiPageType
ms.openlocfilehash: b9f2bdd93c331126ce1155344b44e59802e475b1
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292648"
---
# <a name="get-drive"></a><span data-ttu-id="2ee75-103">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="2ee75-103">Get Drive</span></span>

<span data-ttu-id="2ee75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ee75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ee75-105">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="2ee75-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="2ee75-106">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2ee75-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ee75-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ee75-107">Permissions</span></span>

<span data-ttu-id="2ee75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ee75-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ee75-110">Permission type</span></span>      | <span data-ttu-id="2ee75-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ee75-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ee75-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ee75-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ee75-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee75-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ee75-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ee75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ee75-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee75-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ee75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ee75-116">Application</span></span> | <span data-ttu-id="2ee75-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee75-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="2ee75-118">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="2ee75-118">Get current user's OneDrive</span></span>

<span data-ttu-id="2ee75-119">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="2ee75-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="2ee75-120">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="2ee75-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="2ee75-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee75-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="2ee75-123">C#</span><span class="sxs-lookup"><span data-stu-id="2ee75-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ee75-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee75-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee75-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee75-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee75-126">Java</span><span class="sxs-lookup"><span data-stu-id="2ee75-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="2ee75-127">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="2ee75-127">Get a user's OneDrive</span></span>

<span data-ttu-id="2ee75-128">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="2ee75-128">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="2ee75-129">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="2ee75-129">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="2ee75-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-130">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee75-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="2ee75-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ee75-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ee75-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee75-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee75-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee75-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee75-135">Java</span><span class="sxs-lookup"><span data-stu-id="2ee75-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="2ee75-136">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2ee75-136">Path parameters</span></span>

| <span data-ttu-id="2ee75-137">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ee75-137">Parameter name</span></span> | <span data-ttu-id="2ee75-138">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee75-138">Value</span></span>  | <span data-ttu-id="2ee75-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee75-139">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2ee75-140">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="2ee75-140">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="2ee75-141">string</span><span class="sxs-lookup"><span data-stu-id="2ee75-141">string</span></span> | <span data-ttu-id="2ee75-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee75-142">Required.</span></span> <span data-ttu-id="2ee75-143">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2ee75-143">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="2ee75-144">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="2ee75-144">Get the document library associated with a group</span></span>

<span data-ttu-id="2ee75-145">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="2ee75-145">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="2ee75-146">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-146">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee75-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="2ee75-148">C#</span><span class="sxs-lookup"><span data-stu-id="2ee75-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ee75-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee75-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee75-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee75-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee75-151">Java</span><span class="sxs-lookup"><span data-stu-id="2ee75-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="2ee75-152">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2ee75-152">Path parameters</span></span>

| <span data-ttu-id="2ee75-153">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ee75-153">Parameter name</span></span> | <span data-ttu-id="2ee75-154">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee75-154">Value</span></span>  | <span data-ttu-id="2ee75-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee75-155">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2ee75-156">_groupId_</span><span class="sxs-lookup"><span data-stu-id="2ee75-156">_groupId_</span></span>      | <span data-ttu-id="2ee75-157">string</span><span class="sxs-lookup"><span data-stu-id="2ee75-157">string</span></span> | <span data-ttu-id="2ee75-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee75-158">Required.</span></span> <span data-ttu-id="2ee75-159">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="2ee75-159">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="2ee75-160">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="2ee75-160">Get the document library for a site</span></span>

<span data-ttu-id="2ee75-161">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="2ee75-161">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="2ee75-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-162">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee75-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-163">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="2ee75-164">C#</span><span class="sxs-lookup"><span data-stu-id="2ee75-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ee75-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee75-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee75-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee75-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee75-167">Java</span><span class="sxs-lookup"><span data-stu-id="2ee75-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="2ee75-168">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2ee75-168">Path parameters</span></span>

| <span data-ttu-id="2ee75-169">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ee75-169">Parameter name</span></span> | <span data-ttu-id="2ee75-170">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee75-170">Value</span></span>  | <span data-ttu-id="2ee75-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee75-171">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2ee75-172">_siteId_</span><span class="sxs-lookup"><span data-stu-id="2ee75-172">_siteId_</span></span>       | <span data-ttu-id="2ee75-173">string</span><span class="sxs-lookup"><span data-stu-id="2ee75-173">string</span></span> | <span data-ttu-id="2ee75-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ee75-174">Required.</span></span> <span data-ttu-id="2ee75-175">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="2ee75-175">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="2ee75-176">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="2ee75-176">Get a drive by ID</span></span>

<span data-ttu-id="2ee75-177">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="2ee75-177">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="2ee75-178">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-178">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ee75-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee75-179">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}
```
# <a name="c"></a>[<span data-ttu-id="2ee75-180">C#</span><span class="sxs-lookup"><span data-stu-id="2ee75-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ee75-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ee75-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ee75-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ee75-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ee75-183">Java</span><span class="sxs-lookup"><span data-stu-id="2ee75-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="2ee75-184">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2ee75-184">Path parameters</span></span>

| <span data-ttu-id="2ee75-185">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="2ee75-185">Parameter name</span></span> | <span data-ttu-id="2ee75-186">Valor</span><span class="sxs-lookup"><span data-stu-id="2ee75-186">Value</span></span>  | <span data-ttu-id="2ee75-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee75-187">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="2ee75-188">_driveId_</span><span class="sxs-lookup"><span data-stu-id="2ee75-188">_driveId_</span></span>      | <span data-ttu-id="2ee75-189">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ee75-189">string</span></span> | <span data-ttu-id="2ee75-p105">Obrigatório. O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="2ee75-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2ee75-192">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ee75-192">Optional query parameters</span></span>

<span data-ttu-id="2ee75-193">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee75-193">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="2ee75-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ee75-194">Response</span></span>

<span data-ttu-id="2ee75-195">Cada um desses métodos retorna um [Recurso de Unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ee75-195">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="2ee75-196">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="2ee75-196">Error response codes</span></span>

<span data-ttu-id="2ee75-197">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="2ee75-197">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Microsoft 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": "Drives/Get drive"
} -->

