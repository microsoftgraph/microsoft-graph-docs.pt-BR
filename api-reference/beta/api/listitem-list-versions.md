---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Obtenha uma versão anterior de um registro de lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b8a9078bb0e56f3c3068a92bab9835f2a4964f79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540958"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="fe04f-102">Listar versões de um item de lista (prévia)</span><span class="sxs-lookup"><span data-stu-id="fe04f-102">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe04f-103">O SharePoint pode ser configurado para manter o histórico para itens da lista.</span><span class="sxs-lookup"><span data-stu-id="fe04f-103">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="fe04f-104">Versões anteriores podem ser mantidas por um determinado período dependendo das configurações de administração que podem ser exclusivas por usuário ou local.</span><span class="sxs-lookup"><span data-stu-id="fe04f-104">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe04f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe04f-105">Permissions</span></span>

<span data-ttu-id="fe04f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe04f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="fe04f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe04f-108">Permission type</span></span>             | <span data-ttu-id="fe04f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe04f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fe04f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe04f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe04f-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe04f-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="fe04f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe04f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe04f-113">n/d</span><span class="sxs-lookup"><span data-stu-id="fe04f-113">n/a</span></span>                                         |
| <span data-ttu-id="fe04f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe04f-114">Application</span></span>                            | <span data-ttu-id="fe04f-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe04f-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="fe04f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe04f-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="fe04f-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe04f-117">Response</span></span>

<span data-ttu-id="fe04f-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ListItemVersion](../resources/listitemversion.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe04f-118">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="fe04f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe04f-119">Example</span></span>

<span data-ttu-id="fe04f-120">Este exemplo recupera as versões de um listItem em uma lista do SharePoint:</span><span class="sxs-lookup"><span data-stu-id="fe04f-120">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="fe04f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe04f-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="fe04f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe04f-122">Response</span></span>

<span data-ttu-id="fe04f-123">Isso retornará uma coleção de versões:</span><span class="sxs-lookup"><span data-stu-id="fe04f-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list-versions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
