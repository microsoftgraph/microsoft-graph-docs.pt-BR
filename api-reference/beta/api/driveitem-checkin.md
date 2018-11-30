---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Fazer Check-In de arquivos
ms.openlocfilehash: 49ff3d52ae95cfbe11defbddc0959e8fd8ab7fa6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035320"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="8340c-102">Alterações de check-in em um recurso de DriveItem</span><span class="sxs-lookup"><span data-stu-id="8340c-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="8340c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8340c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8340c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8340c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8340c-105">Check-in de um recurso DriveItem com check-out, que disponibiliza a versão do documento para outras pessoas.</span><span class="sxs-lookup"><span data-stu-id="8340c-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="8340c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8340c-106">Permissions</span></span>

<span data-ttu-id="8340c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8340c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8340c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8340c-109">Permission type</span></span>      | <span data-ttu-id="8340c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8340c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8340c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8340c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8340c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8340c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8340c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8340c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8340c-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8340c-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8340c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8340c-115">Application</span></span> | <span data-ttu-id="8340c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8340c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8340c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8340c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="8340c-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8340c-118">Request body</span></span>

<span data-ttu-id="8340c-119">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8340c-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="8340c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8340c-120">Name</span></span>    | <span data-ttu-id="8340c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8340c-121">Value</span></span>  |                                                <span data-ttu-id="8340c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8340c-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8340c-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="8340c-123">checkInAs</span></span> | <span data-ttu-id="8340c-124">string</span><span class="sxs-lookup"><span data-stu-id="8340c-124">string</span></span> | <span data-ttu-id="8340c-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8340c-125">Optional.</span></span> <span data-ttu-id="8340c-126">O status desejado do documento após a conclusão da operação de check-in.</span><span class="sxs-lookup"><span data-stu-id="8340c-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="8340c-127">Pode ser `published` ou não especificado.</span><span class="sxs-lookup"><span data-stu-id="8340c-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="8340c-128">comment</span><span class="sxs-lookup"><span data-stu-id="8340c-128">comment</span></span>   | <span data-ttu-id="8340c-129">string</span><span class="sxs-lookup"><span data-stu-id="8340c-129">string</span></span> | <span data-ttu-id="8340c-130">Um comentário de check-in comentário associado à versão.</span><span class="sxs-lookup"><span data-stu-id="8340c-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="8340c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8340c-131">Example</span></span>

<span data-ttu-id="8340c-132">Este exemplo faz check-in de um arquivo identificado por `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="8340c-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="8340c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8340c-133">Response</span></span>

<span data-ttu-id="8340c-134">Se tiver êxito, a chamada API retorna um código `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="8340c-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="8340c-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="8340c-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
