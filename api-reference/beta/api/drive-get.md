---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter Unidade
ms.openlocfilehash: 903eb9d5886bf2ec3b7f8672438f01482e754f9b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748588"
---
# <a name="get-drive"></a><span data-ttu-id="08f3a-102">Obter Unidade</span><span class="sxs-lookup"><span data-stu-id="08f3a-102">Get Drive</span></span>

> <span data-ttu-id="08f3a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="08f3a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08f3a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="08f3a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08f3a-105">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="08f3a-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="08f3a-106">Uma unidade é um contêiner de nível superior para um sistema de arquivos como as bibliotecas de documentos do OneDrive ou do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="08f3a-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="08f3a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08f3a-107">Permissions</span></span>

<span data-ttu-id="08f3a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08f3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08f3a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08f3a-110">Permission type</span></span>      | <span data-ttu-id="08f3a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08f3a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08f3a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08f3a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08f3a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f3a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="08f3a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08f3a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08f3a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f3a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="08f3a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08f3a-116">Application</span></span> | <span data-ttu-id="08f3a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f3a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="08f3a-118">Obter o OneDrive do usuário atual</span><span class="sxs-lookup"><span data-stu-id="08f3a-118">Get current user's OneDrive</span></span>

<span data-ttu-id="08f3a-119">A unidade do usuário conectado (ao usar a autenticação delegada) poderá ser acessada pelo `me` singleton.</span><span class="sxs-lookup"><span data-stu-id="08f3a-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="08f3a-120">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="08f3a-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="08f3a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08f3a-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="08f3a-122">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="08f3a-122">Get a user's OneDrive</span></span>

<span data-ttu-id="08f3a-123">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso User.</span><span class="sxs-lookup"><span data-stu-id="08f3a-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="08f3a-124">Se o OneDrive do usuário não está provisionado, mas o usuário tem uma licença para usar o OneDrive, esta solicitação provisionará automaticamente ao usar a autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="08f3a-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="08f3a-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08f3a-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="08f3a-126">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="08f3a-126">Path parameters</span></span>

| <span data-ttu-id="08f3a-127">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="08f3a-127">Parameter name</span></span> | <span data-ttu-id="08f3a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="08f3a-128">Value</span></span>  | <span data-ttu-id="08f3a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="08f3a-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="08f3a-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="08f3a-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="08f3a-131">string</span><span class="sxs-lookup"><span data-stu-id="08f3a-131">string</span></span> | <span data-ttu-id="08f3a-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08f3a-132">Required.</span></span> <span data-ttu-id="08f3a-133">O identificador de objeto do usuário proprietário do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="08f3a-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="08f3a-134">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="08f3a-134">Get the document library associated with a group</span></span>

<span data-ttu-id="08f3a-135">Para acessar uma biblioteca de documentos padrão de um Grupo, o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="08f3a-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="08f3a-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08f3a-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="08f3a-137">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="08f3a-137">Path parameters</span></span>

| <span data-ttu-id="08f3a-138">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="08f3a-138">Parameter name</span></span> | <span data-ttu-id="08f3a-139">Valor</span><span class="sxs-lookup"><span data-stu-id="08f3a-139">Value</span></span>  | <span data-ttu-id="08f3a-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="08f3a-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="08f3a-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="08f3a-141">_groupId_</span></span>      | <span data-ttu-id="08f3a-142">string</span><span class="sxs-lookup"><span data-stu-id="08f3a-142">string</span></span> | <span data-ttu-id="08f3a-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08f3a-143">Required.</span></span> <span data-ttu-id="08f3a-144">O identificador do grupo proprietário da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="08f3a-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="08f3a-145">Obter a biblioteca de documentos de um site</span><span class="sxs-lookup"><span data-stu-id="08f3a-145">Get the document library for a site</span></span>

<span data-ttu-id="08f3a-146">Para acessar uma biblioteca de documentos padrão [de um Site](../resources/site.md), o aplicativo solicita a relação **drive** no Site.</span><span class="sxs-lookup"><span data-stu-id="08f3a-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="08f3a-147">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08f3a-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="08f3a-148">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="08f3a-148">Path parameters</span></span>

| <span data-ttu-id="08f3a-149">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="08f3a-149">Parameter name</span></span> | <span data-ttu-id="08f3a-150">Valor</span><span class="sxs-lookup"><span data-stu-id="08f3a-150">Value</span></span>  | <span data-ttu-id="08f3a-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="08f3a-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="08f3a-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="08f3a-152">_siteId_</span></span>       | <span data-ttu-id="08f3a-153">string</span><span class="sxs-lookup"><span data-stu-id="08f3a-153">string</span></span> | <span data-ttu-id="08f3a-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08f3a-154">Required.</span></span> <span data-ttu-id="08f3a-155">O identificador do site que contém a biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="08f3a-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="08f3a-156">Obtenha uma unidade por ID</span><span class="sxs-lookup"><span data-stu-id="08f3a-156">Get a drive by ID</span></span>

<span data-ttu-id="08f3a-157">Se tiver o identificador exclusivo de uma unidade, você poderá acessá-lo diretamente da coleção de unidades de nível superior.</span><span class="sxs-lookup"><span data-stu-id="08f3a-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="08f3a-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08f3a-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="08f3a-159">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="08f3a-159">Path parameters</span></span>

| <span data-ttu-id="08f3a-160">Nome do parâmetro</span><span class="sxs-lookup"><span data-stu-id="08f3a-160">Parameter name</span></span> | <span data-ttu-id="08f3a-161">Valor</span><span class="sxs-lookup"><span data-stu-id="08f3a-161">Value</span></span>  | <span data-ttu-id="08f3a-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="08f3a-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="08f3a-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="08f3a-163">_driveId_</span></span>      | <span data-ttu-id="08f3a-164">string</span><span class="sxs-lookup"><span data-stu-id="08f3a-164">string</span></span> | <span data-ttu-id="08f3a-165">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08f3a-165">Required.</span></span> <span data-ttu-id="08f3a-166">O identificador da unidade solicitada.</span><span class="sxs-lookup"><span data-stu-id="08f3a-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="08f3a-167">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08f3a-167">Optional query parameters</span></span>

<span data-ttu-id="08f3a-168">Esse método é compatível com o [parâmetro de consulta $select][odata-query-parameters] para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08f3a-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="08f3a-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="08f3a-169">Response</span></span>

<span data-ttu-id="08f3a-170">Cada um desses métodos retorna um [recurso de unidade][drive-resource] para a unidade correspondente no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08f3a-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="08f3a-171">Códigos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="08f3a-171">Error response codes</span></span>

<span data-ttu-id="08f3a-172">Se a unidade não existir e não puder ser provisionada automaticamente (ao usar autenticação delegada) uma resposta `HTTP 404` será retornada.</span><span class="sxs-lookup"><span data-stu-id="08f3a-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
