---
author: JeremyKelley
description: Recupera a lista de recursos Drive disponíveis para um User, Group ou Site de destino.
ms.date: 09/10/2017
title: Listar unidades
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 319a0b18952b13de329aabccc222f01bdbf02e18
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982231"
---
# <a name="list-available-drives"></a><span data-ttu-id="3dc05-103">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="3dc05-103">List available drives</span></span>

<span data-ttu-id="3dc05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dc05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dc05-105">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.</span><span class="sxs-lookup"><span data-stu-id="3dc05-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3dc05-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dc05-106">Permissions</span></span>

<span data-ttu-id="3dc05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dc05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dc05-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dc05-109">Permission type</span></span>      | <span data-ttu-id="3dc05-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dc05-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dc05-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dc05-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3dc05-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc05-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dc05-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dc05-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dc05-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc05-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dc05-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dc05-115">Application</span></span> | <span data-ttu-id="3dc05-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc05-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="3dc05-117">Lista as unidades de um grupo</span><span class="sxs-lookup"><span data-stu-id="3dc05-117">List a group's drives</span></span>

<span data-ttu-id="3dc05-118">Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.</span><span class="sxs-lookup"><span data-stu-id="3dc05-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="3dc05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc05-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc05-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc05-120">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drives
```
# <a name="c"></a>[<span data-ttu-id="3dc05-121">C#</span><span class="sxs-lookup"><span data-stu-id="3dc05-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc05-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc05-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc05-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc05-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="3dc05-124">Lista as unidades do site</span><span class="sxs-lookup"><span data-stu-id="3dc05-124">List a site's drives</span></span>

<span data-ttu-id="3dc05-125">Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.</span><span class="sxs-lookup"><span data-stu-id="3dc05-125">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc05-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc05-126">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drives
```
# <a name="c"></a>[<span data-ttu-id="3dc05-127">C#</span><span class="sxs-lookup"><span data-stu-id="3dc05-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc05-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc05-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc05-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc05-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="3dc05-130">Lista as unidades de um usuário</span><span class="sxs-lookup"><span data-stu-id="3dc05-130">List a user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc05-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc05-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{userId}/drives
```
# <a name="c"></a>[<span data-ttu-id="3dc05-132">C#</span><span class="sxs-lookup"><span data-stu-id="3dc05-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc05-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc05-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc05-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc05-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="3dc05-135">Lista as unidades do usuário atual</span><span class="sxs-lookup"><span data-stu-id="3dc05-135">List the current user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="3dc05-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3dc05-136">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drives
```
# <a name="c"></a>[<span data-ttu-id="3dc05-137">C#</span><span class="sxs-lookup"><span data-stu-id="3dc05-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3dc05-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3dc05-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3dc05-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3dc05-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="3dc05-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3dc05-140">Optional query parameters</span></span>

<span data-ttu-id="3dc05-141">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="3dc05-141">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="3dc05-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dc05-142">Response</span></span>

<span data-ttu-id="3dc05-143">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dc05-143">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="3dc05-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="3dc05-144">Remarks</span></span>

<span data-ttu-id="3dc05-145">A maioria dos usuários só terá um único recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="3dc05-145">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="3dc05-146">Grupos e Sites podem ter vários recursos de unidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="3dc05-146">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="3dc05-147">Unidades com a faceta [sistema][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="3dc05-147">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="3dc05-148">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="3dc05-148">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
}
-->


