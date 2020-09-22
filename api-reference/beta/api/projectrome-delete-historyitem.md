---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 1fa3b1863445caa5ce7a953a98d12310b4abeec9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017301"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="1e5e7-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="1e5e7-103">Delete a historyItem</span></span>

<span data-ttu-id="1e5e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e5e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e5e7-105">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e5e7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e5e7-106">Permissions</span></span>

<span data-ttu-id="1e5e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e5e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1e5e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e5e7-109">Permission type</span></span>      | <span data-ttu-id="1e5e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e5e7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e5e7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e5e7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e5e7-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1e5e7-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1e5e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e5e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e5e7-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1e5e7-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1e5e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e5e7-115">Application</span></span> | <span data-ttu-id="1e5e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e5e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e5e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e5e7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5e7-118">Request headers</span></span>

|<span data-ttu-id="1e5e7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1e5e7-119">Name</span></span> | <span data-ttu-id="1e5e7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5e7-120">Type</span></span> | <span data-ttu-id="1e5e7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5e7-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1e5e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e5e7-122">Authorization</span></span> | <span data-ttu-id="1e5e7-123">string</span><span class="sxs-lookup"><span data-stu-id="1e5e7-123">string</span></span> | <span data-ttu-id="1e5e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e5e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5e7-126">Request body</span></span>

<span data-ttu-id="1e5e7-127">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1e5e7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5e7-128">Response</span></span>

<span data-ttu-id="1e5e7-129">Se tiver êxito, este método retornará o `204 No Content` código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="1e5e7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e5e7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1e5e7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e5e7-131">Request</span></span>

<span data-ttu-id="1e5e7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1e5e7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e5e7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```
# <a name="objective-c"></a>[<span data-ttu-id="1e5e7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e5e7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1e5e7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e5e7-135">Response</span></span>

<span data-ttu-id="1e5e7-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e5e7-136">Here is an example of the response.</span></span>

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
  "suppressions": [
  ]
}
-->


