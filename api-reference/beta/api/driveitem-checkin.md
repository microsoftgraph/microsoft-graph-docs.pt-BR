---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Check-in de arquivos
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cec932eef89c02569d6f350f436c6a7721286e92
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325400"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="356ba-102">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="356ba-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356ba-103">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="356ba-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="356ba-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="356ba-104">Permissions</span></span>

<span data-ttu-id="356ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356ba-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="356ba-107">Permission type</span></span>      | <span data-ttu-id="356ba-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="356ba-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356ba-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="356ba-109">Delegated (work or school account)</span></span> | <span data-ttu-id="356ba-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356ba-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="356ba-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="356ba-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356ba-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356ba-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="356ba-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="356ba-113">Application</span></span> | <span data-ttu-id="356ba-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356ba-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356ba-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="356ba-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="356ba-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="356ba-116">Request body</span></span>

<span data-ttu-id="356ba-117">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="356ba-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="356ba-118">Nome</span><span class="sxs-lookup"><span data-stu-id="356ba-118">Name</span></span>    | <span data-ttu-id="356ba-119">Valor</span><span class="sxs-lookup"><span data-stu-id="356ba-119">Value</span></span>  |                                                <span data-ttu-id="356ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="356ba-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="356ba-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="356ba-121">checkInAs</span></span> | <span data-ttu-id="356ba-122">string</span><span class="sxs-lookup"><span data-stu-id="356ba-122">string</span></span> | <span data-ttu-id="356ba-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="356ba-123">Optional.</span></span> <span data-ttu-id="356ba-124">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="356ba-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="356ba-125">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="356ba-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="356ba-126">comment</span><span class="sxs-lookup"><span data-stu-id="356ba-126">comment</span></span>   | <span data-ttu-id="356ba-127">string</span><span class="sxs-lookup"><span data-stu-id="356ba-127">string</span></span> | <span data-ttu-id="356ba-128">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="356ba-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="356ba-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="356ba-129">Example</span></span>

<span data-ttu-id="356ba-130">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="356ba-130">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="356ba-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="356ba-131">Response</span></span>

<span data-ttu-id="356ba-132">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="356ba-132">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="356ba-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="356ba-133">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
