---
author: learafa
description: Faça check-in em um recurso de driveItem com check-out, que torna a versão do documento disponível para outras pessoas.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6a48578b3b823f881b5f34e5d18a169f595d038d
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227754"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="337ce-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="337ce-103">driveItem: checkin</span></span>

<span data-ttu-id="337ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="337ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="337ce-105">Faça check-in em um recurso de **driveItem** com check-out, que torna a versão do documento disponível para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="337ce-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="337ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="337ce-106">Permissions</span></span>

<span data-ttu-id="337ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="337ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="337ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="337ce-109">Permission type</span></span>      | <span data-ttu-id="337ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="337ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="337ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="337ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="337ce-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337ce-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="337ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="337ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="337ce-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337ce-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="337ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="337ce-115">Application</span></span> | <span data-ttu-id="337ce-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337ce-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="337ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="337ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

## <a name="request-body"></a><span data-ttu-id="337ce-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="337ce-118">Request body</span></span>

<span data-ttu-id="337ce-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="337ce-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="337ce-120">Nome</span><span class="sxs-lookup"><span data-stu-id="337ce-120">Name</span></span>    | <span data-ttu-id="337ce-121">Valor</span><span class="sxs-lookup"><span data-stu-id="337ce-121">Value</span></span>  |                                                <span data-ttu-id="337ce-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="337ce-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="337ce-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="337ce-123">checkInAs</span></span> | <span data-ttu-id="337ce-124">string</span><span class="sxs-lookup"><span data-stu-id="337ce-124">string</span></span> | <span data-ttu-id="337ce-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="337ce-125">Optional.</span></span> <span data-ttu-id="337ce-126">O status do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="337ce-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="337ce-127">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="337ce-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="337ce-128">comment</span><span class="sxs-lookup"><span data-stu-id="337ce-128">comment</span></span>   | <span data-ttu-id="337ce-129">string</span><span class="sxs-lookup"><span data-stu-id="337ce-129">string</span></span> | <span data-ttu-id="337ce-130">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="337ce-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="response"></a><span data-ttu-id="337ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="337ce-131">Response</span></span>

<span data-ttu-id="337ce-132">Se tiver êxito, a chamada de `204 No content`API retornará.</span><span class="sxs-lookup"><span data-stu-id="337ce-132">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="337ce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="337ce-133">Example</span></span>

<span data-ttu-id="337ce-134">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="337ce-134">This example checks in a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="337ce-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="337ce-135">Request</span></span>
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

### <a name="response"></a><span data-ttu-id="337ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="337ce-136">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
