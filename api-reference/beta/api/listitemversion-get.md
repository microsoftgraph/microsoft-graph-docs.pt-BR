---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obter uma versão anterior de um item de lista - API do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2193c2e23ad5227e9118f23a782fbaa24756f88b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338702"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="1efd9-102">Obter um recurso ListItemVersion (prévia)</span><span class="sxs-lookup"><span data-stu-id="1efd9-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1efd9-103">Recuperar os metadados de uma versão específica de um [ListItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="1efd9-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1efd9-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="1efd9-104">Permissions</span></span>

<span data-ttu-id="1efd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1efd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="1efd9-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1efd9-107">Permission type</span></span>             | <span data-ttu-id="1efd9-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1efd9-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1efd9-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1efd9-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1efd9-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1efd9-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="1efd9-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1efd9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1efd9-112">n/d</span><span class="sxs-lookup"><span data-stu-id="1efd9-112">n/a</span></span>                                         |
| <span data-ttu-id="1efd9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1efd9-113">Application</span></span>                            | <span data-ttu-id="1efd9-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1efd9-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="1efd9-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1efd9-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="1efd9-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efd9-116">Response</span></span>

<span data-ttu-id="1efd9-117">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1efd9-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="1efd9-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1efd9-118">Example</span></span>

<span data-ttu-id="1efd9-119">Este exemplo recupera uma versão de um item de lista e expande o conjunto de campos para solicitar os valores dos campos no listItem.</span><span class="sxs-lookup"><span data-stu-id="1efd9-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="1efd9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1efd9-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="1efd9-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="1efd9-121">Response</span></span>

<span data-ttu-id="1efd9-122">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="1efd9-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": []
}
-->
