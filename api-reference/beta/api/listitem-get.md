---
author: JeremyKelley
description: Retorna os metadados de um item em uma lista.
ms.date: 09/11/2017
title: Obter uma entrada de uma lista do SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d3d2e431bfa73e92fd99a146ad9820b46d21b4dc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475847"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="a89b1-103">Obter um item em uma lista</span><span class="sxs-lookup"><span data-stu-id="a89b1-103">Get an item in a list</span></span>

<span data-ttu-id="a89b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89b1-105">Retorna os metadados de um [item][] em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="a89b1-105">Returns the metadata for an [item][] in a [list][].</span></span>

[lista]: ../resources/list.md
[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="a89b1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a89b1-108">Permissions</span></span>

<span data-ttu-id="a89b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89b1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a89b1-111">Permission type</span></span>      | <span data-ttu-id="a89b1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a89b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89b1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a89b1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a89b1-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89b1-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="a89b1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a89b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89b1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a89b1-116">Not supported.</span></span>    |
|<span data-ttu-id="a89b1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a89b1-117">Application</span></span> | <span data-ttu-id="a89b1-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a89b1-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="a89b1-119">**Observação**: a permissão do aplicativo Sites.Manage.All será necessária se a lista do SharePoint tiver as configurações de aprovação de conteúdo ativadas.</span><span class="sxs-lookup"><span data-stu-id="a89b1-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="a89b1-120">Caso contrário, o Microsoft Graph não recuperará itens de lista que tenham um status de aprovação diferente de Aprovado.</span><span class="sxs-lookup"><span data-stu-id="a89b1-120">Otherwise, Microsoft Graph won't retrieve list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="a89b1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a89b1-121">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a89b1-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a89b1-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a89b1-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a89b1-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a89b1-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89b1-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="a89b1-125">C#</span><span class="sxs-lookup"><span data-stu-id="a89b1-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a89b1-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a89b1-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a89b1-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a89b1-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a89b1-128">Java</span><span class="sxs-lookup"><span data-stu-id="a89b1-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a89b1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a89b1-129">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->


