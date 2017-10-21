---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Criar uma nova entrada em uma lista do SharePoint
ms.openlocfilehash: 55a3c52d7afb2a276055cdddfb826ebbcb574ae7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="446ca-102">Criar um novo item em uma lista</span><span class="sxs-lookup"><span data-stu-id="446ca-102">Create a new item in a list</span></span>

<span data-ttu-id="446ca-103">Criar um novo [listItem][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="446ca-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="446ca-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="446ca-104">Permissions</span></span>

<span data-ttu-id="446ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="446ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="446ca-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="446ca-107">Permission type</span></span>      | <span data-ttu-id="446ca-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="446ca-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="446ca-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="446ca-109">Delegated (work or school account)</span></span> | <span data-ttu-id="446ca-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446ca-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="446ca-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="446ca-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="446ca-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="446ca-112">Not supported.</span></span>    |
|<span data-ttu-id="446ca-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="446ca-113">Application</span></span> | <span data-ttu-id="446ca-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="446ca-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="446ca-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="446ca-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="446ca-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="446ca-116">Request body</span></span>

<span data-ttu-id="446ca-117">No corpo da solicitação, forneça uma representação JSON do recurso [listItem][] a criar.</span><span class="sxs-lookup"><span data-stu-id="446ca-117">In the request body, supply a JSON representation of the [DriveItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="446ca-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="446ca-118">Example</span></span>

<span data-ttu-id="446ca-119">Aqui está um exemplo de como criar um novo item de lista genérica.</span><span class="sxs-lookup"><span data-stu-id="446ca-119">Here is an example of how to create a new folder.</span></span>

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

## <a name="response"></a><span data-ttu-id="446ca-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="446ca-120">Response</span></span>

<span data-ttu-id="446ca-121">Se for bem-sucedido, esse método retornará um [listItem][] no corpo da resposta da lista criada.</span><span class="sxs-lookup"><span data-stu-id="446ca-121">If successful, this method returns a [driveItem][] object in the response body for the newly created file.</span></span>

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

<span data-ttu-id="446ca-122">**Observação:** O objeto Response será truncado para mais clareza.</span><span class="sxs-lookup"><span data-stu-id="446ca-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="446ca-123">As propriedades padrão serão retornadas da chamada real.</span><span class="sxs-lookup"><span data-stu-id="446ca-123">All default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listItem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
