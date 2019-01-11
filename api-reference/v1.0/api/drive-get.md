---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter Unidade
localization_priority: Priority
ms.openlocfilehash: ffa7162b700fc4f3e9a13b98ca3cef501d870291
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846309"
---
# <a name="get-drive"></a><span data-ttu-id="07f0f-102">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="07f0f-102">Get Drive</span></span>

<span data-ttu-id="07f0f-103">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="07f0f-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="07f0f-104">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07f0f-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="07f0f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="07f0f-105">Permissions</span></span>

<span data-ttu-id="07f0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f0f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07f0f-108">Permission type</span></span>      | <span data-ttu-id="07f0f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07f0f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07f0f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07f0f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07f0f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f0f-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="07f0f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07f0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07f0f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f0f-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="07f0f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07f0f-114">Application</span></span> | <span data-ttu-id="07f0f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f0f-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="07f0f-116">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="07f0f-116">Get current user's OneDrive</span></span>

<span data-ttu-id="07f0f-117">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="07f0f-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="07f0f-118">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="07f0f-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="07f0f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f0f-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="07f0f-120">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="07f0f-120">Get a user's OneDrive</span></span>

<span data-ttu-id="07f0f-121">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="07f0f-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="07f0f-122">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="07f0f-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="07f0f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f0f-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="07f0f-124">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="07f0f-124">Path parameters</span></span>

| <span data-ttu-id="07f0f-125">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="07f0f-125">Parameter name</span></span> | <span data-ttu-id="07f0f-126">Valor</span><span class="sxs-lookup"><span data-stu-id="07f0f-126">Value</span></span>  | <span data-ttu-id="07f0f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="07f0f-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="07f0f-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="07f0f-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="07f0f-129">string</span><span class="sxs-lookup"><span data-stu-id="07f0f-129">string</span></span> | <span data-ttu-id="07f0f-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07f0f-130">Required.</span></span> <span data-ttu-id="07f0f-131">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="07f0f-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="07f0f-132">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="07f0f-132">Get the document library associated with a group</span></span>

<span data-ttu-id="07f0f-133">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="07f0f-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="07f0f-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f0f-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="07f0f-135">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="07f0f-135">Path parameters</span></span>

| <span data-ttu-id="07f0f-136">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="07f0f-136">Parameter name</span></span> | <span data-ttu-id="07f0f-137">Valor</span><span class="sxs-lookup"><span data-stu-id="07f0f-137">Value</span></span>  | <span data-ttu-id="07f0f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="07f0f-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="07f0f-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="07f0f-139">_groupId_</span></span>      | <span data-ttu-id="07f0f-140">string</span><span class="sxs-lookup"><span data-stu-id="07f0f-140">string</span></span> | <span data-ttu-id="07f0f-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07f0f-141">Required.</span></span> <span data-ttu-id="07f0f-142">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="07f0f-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="07f0f-143">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="07f0f-143">Get the document library for a site</span></span>

<span data-ttu-id="07f0f-144">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="07f0f-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="07f0f-145">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f0f-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="07f0f-146">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="07f0f-146">Path parameters</span></span>

| <span data-ttu-id="07f0f-147">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="07f0f-147">Parameter name</span></span> | <span data-ttu-id="07f0f-148">Valor</span><span class="sxs-lookup"><span data-stu-id="07f0f-148">Value</span></span>  | <span data-ttu-id="07f0f-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="07f0f-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="07f0f-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="07f0f-150">_siteId_</span></span>       | <span data-ttu-id="07f0f-151">string</span><span class="sxs-lookup"><span data-stu-id="07f0f-151">string</span></span> | <span data-ttu-id="07f0f-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07f0f-152">Required.</span></span> <span data-ttu-id="07f0f-153">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="07f0f-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="07f0f-154">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="07f0f-154">Get a drive by ID</span></span>

<span data-ttu-id="07f0f-155">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="07f0f-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="07f0f-156">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f0f-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="07f0f-157">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="07f0f-157">Path parameters</span></span>

| <span data-ttu-id="07f0f-158">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="07f0f-158">Parameter name</span></span> | <span data-ttu-id="07f0f-159">Valor</span><span class="sxs-lookup"><span data-stu-id="07f0f-159">Value</span></span>  | <span data-ttu-id="07f0f-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="07f0f-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="07f0f-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="07f0f-161">_driveId_</span></span>      | <span data-ttu-id="07f0f-162">string</span><span class="sxs-lookup"><span data-stu-id="07f0f-162">string</span></span> | <span data-ttu-id="07f0f-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07f0f-163">Required.</span></span> <span data-ttu-id="07f0f-164">O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="07f0f-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="07f0f-165">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="07f0f-165">Optional query parameters</span></span>

<span data-ttu-id="07f0f-166">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="07f0f-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="07f0f-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="07f0f-167">Response</span></span>

<span data-ttu-id="07f0f-168">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07f0f-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="07f0f-169">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="07f0f-169">Error response codes</span></span>

<span data-ttu-id="07f0f-170">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="07f0f-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
