---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 0e55b38b2db41b5ecd92bd8dee5ba8e0559ba745
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337199"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="b16fd-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="b16fd-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b16fd-104">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="b16fd-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="b16fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b16fd-105">Permissions</span></span>

<span data-ttu-id="b16fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b16fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b16fd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b16fd-108">Permission type</span></span>      | <span data-ttu-id="b16fd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b16fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b16fd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b16fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b16fd-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b16fd-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b16fd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b16fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b16fd-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b16fd-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b16fd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b16fd-114">Application</span></span> | <span data-ttu-id="b16fd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b16fd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b16fd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b16fd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b16fd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b16fd-117">Request headers</span></span>

|<span data-ttu-id="b16fd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b16fd-118">Name</span></span> | <span data-ttu-id="b16fd-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b16fd-119">Type</span></span> | <span data-ttu-id="b16fd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b16fd-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b16fd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b16fd-121">Authorization</span></span> | <span data-ttu-id="b16fd-122">string</span><span class="sxs-lookup"><span data-stu-id="b16fd-122">string</span></span> | <span data-ttu-id="b16fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b16fd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b16fd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b16fd-125">Request body</span></span>

<span data-ttu-id="b16fd-126">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b16fd-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="b16fd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16fd-127">Response</span></span>

<span data-ttu-id="b16fd-128">Se tiver êxito, este método retornará `204 No Content` o código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="b16fd-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="b16fd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b16fd-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b16fd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b16fd-130">Request</span></span>

<span data-ttu-id="b16fd-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b16fd-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="b16fd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b16fd-132">Response</span></span>

<span data-ttu-id="b16fd-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b16fd-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
