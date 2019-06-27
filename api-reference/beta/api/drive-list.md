---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Listar unidades
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8826d802c6f5507887326dca9fec6b1453485830
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260337"
---
# <a name="list-available-drives"></a><span data-ttu-id="c2de3-102">Listar as unidades disponíveis</span><span class="sxs-lookup"><span data-stu-id="c2de3-102">List available drives</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2de3-103">Recupera a lista de recursos [Drive](../resources/drive.md) disponíveis para um User, Group ou [Site](../resources/site.md) de destino.</span><span class="sxs-lookup"><span data-stu-id="c2de3-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2de3-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2de3-104">Permissions</span></span>

<span data-ttu-id="c2de3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2de3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2de3-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2de3-107">Permission type</span></span>      | <span data-ttu-id="c2de3-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2de3-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2de3-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2de3-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c2de3-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2de3-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2de3-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2de3-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2de3-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2de3-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2de3-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2de3-113">Application</span></span> | <span data-ttu-id="c2de3-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2de3-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="c2de3-115">Lista as unidades de um grupo</span><span class="sxs-lookup"><span data-stu-id="c2de3-115">List a group's drives</span></span>

<span data-ttu-id="c2de3-116">Para listar as bibliotecas de documentos de um grupo, seu aplicativo solicita a relação de **unidades** no Grupo.</span><span class="sxs-lookup"><span data-stu-id="c2de3-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2de3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2de3-117">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2de3-118">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2de3-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2de3-119">C#</span><span class="sxs-lookup"><span data-stu-id="c2de3-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2de3-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2de3-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2de3-121">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2de3-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-sites-drives"></a><span data-ttu-id="c2de3-122">Lista as unidades do site</span><span class="sxs-lookup"><span data-stu-id="c2de3-122">List a site's drives</span></span>

<span data-ttu-id="c2de3-123">Para listar as bibliotecas de documentos de um site, seu aplicativo solicita a relação de **unidades** no Site.</span><span class="sxs-lookup"><span data-stu-id="c2de3-123">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2de3-124">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2de3-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2de3-125">C#</span><span class="sxs-lookup"><span data-stu-id="c2de3-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/site-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2de3-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2de3-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/site-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2de3-127">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2de3-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/site-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-users-drives"></a><span data-ttu-id="c2de3-128">Lista as unidades de um usuário</span><span class="sxs-lookup"><span data-stu-id="c2de3-128">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2de3-129">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2de3-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2de3-130">C#</span><span class="sxs-lookup"><span data-stu-id="c2de3-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2de3-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2de3-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2de3-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2de3-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-the-current-users-drives"></a><span data-ttu-id="c2de3-133">Lista as unidades do usuário atual</span><span class="sxs-lookup"><span data-stu-id="c2de3-133">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2de3-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c2de3-134">Optional query parameters</span></span>

<span data-ttu-id="c2de3-135">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` e `$orderby` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="c2de3-135">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="c2de3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2de3-136">Response</span></span>

<span data-ttu-id="c2de3-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2de3-137">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2de3-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c2de3-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2de3-139">C#</span><span class="sxs-lookup"><span data-stu-id="c2de3-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2de3-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2de3-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2de3-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c2de3-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="c2de3-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2de3-142">Remarks</span></span>

<span data-ttu-id="c2de3-143">A maioria dos usuários só terá um único recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="c2de3-143">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="c2de3-144">Grupos e Sites podem ter vários recursos de unidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c2de3-144">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="c2de3-145">Unidades com a faceta [sistema][] estão ocultas por padrão.</span><span class="sxs-lookup"><span data-stu-id="c2de3-145">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="c2de3-146">Para listá-los, inclua `system` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="c2de3-146">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
