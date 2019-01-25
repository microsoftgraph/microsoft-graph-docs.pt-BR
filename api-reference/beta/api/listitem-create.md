---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 58e008ffc4685348aa8d69f44cbfcf59f4fbf715
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528813"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="90fca-102">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="90fca-102">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90fca-103">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="90fca-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="90fca-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="90fca-104">Permissions</span></span>

<span data-ttu-id="90fca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90fca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90fca-107">Permission type</span></span>      | <span data-ttu-id="90fca-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90fca-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90fca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90fca-109">Delegated (work or school account)</span></span> | <span data-ttu-id="90fca-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fca-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="90fca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90fca-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90fca-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90fca-112">Not supported.</span></span>    |
|<span data-ttu-id="90fca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90fca-113">Application</span></span> | <span data-ttu-id="90fca-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fca-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90fca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90fca-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="90fca-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90fca-116">Request body</span></span>

<span data-ttu-id="90fca-117">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="90fca-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="90fca-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90fca-118">Example</span></span>

<span data-ttu-id="90fca-119">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="90fca-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="90fca-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="90fca-120">Response</span></span>

<span data-ttu-id="90fca-121">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="90fca-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="90fca-122">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="90fca-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="90fca-123">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="90fca-123">Default properties will be returned from the actual call.</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
