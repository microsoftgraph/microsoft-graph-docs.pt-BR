---
title: Excluir um historyItem
description: Exclua um item de histórico existente para uma atividade do usuário existente.
localization_priority: Normal
ms.openlocfilehash: d9468034f3a98e949eeb9f2da28c4a74c42cd991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834976"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="31fdf-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="31fdf-103">Delete a historyItem</span></span>

> <span data-ttu-id="31fdf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31fdf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31fdf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31fdf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31fdf-106">Exclua um item de histórico existente para uma atividade do usuário existente.</span><span class="sxs-lookup"><span data-stu-id="31fdf-106">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="31fdf-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="31fdf-107">Permissions</span></span>

<span data-ttu-id="31fdf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31fdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="31fdf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31fdf-110">Permission type</span></span>      | <span data-ttu-id="31fdf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31fdf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31fdf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31fdf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="31fdf-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="31fdf-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="31fdf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31fdf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31fdf-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="31fdf-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="31fdf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31fdf-116">Application</span></span> | <span data-ttu-id="31fdf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31fdf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31fdf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31fdf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="31fdf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31fdf-119">Request headers</span></span>

|<span data-ttu-id="31fdf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="31fdf-120">Name</span></span> | <span data-ttu-id="31fdf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="31fdf-121">Type</span></span> | <span data-ttu-id="31fdf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="31fdf-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="31fdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31fdf-123">Authorization</span></span> | <span data-ttu-id="31fdf-124">string</span><span class="sxs-lookup"><span data-stu-id="31fdf-124">string</span></span> | <span data-ttu-id="31fdf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31fdf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31fdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31fdf-127">Request body</span></span>

<span data-ttu-id="31fdf-128">Nenhum corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31fdf-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="31fdf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31fdf-129">Response</span></span>

<span data-ttu-id="31fdf-130">Se tiver êxito, este método retornará o `204 No Content` código de resposta se o item de histórico foi excluído.</span><span class="sxs-lookup"><span data-stu-id="31fdf-130">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="31fdf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31fdf-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="31fdf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31fdf-132">Request</span></span>

<span data-ttu-id="31fdf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31fdf-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="31fdf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="31fdf-134">Response</span></span>

<span data-ttu-id="31fdf-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31fdf-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
