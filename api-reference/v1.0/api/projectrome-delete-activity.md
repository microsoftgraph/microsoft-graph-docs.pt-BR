---
title: Excluir uma atividade
description: Excluir uma atividade de usuário existente para seu aplicativo.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: bc739a8f65f477528d603f57427e74734261cfd0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275156"
---
# <a name="delete-an-activity"></a><span data-ttu-id="fa80b-103">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="fa80b-103">Delete an activity</span></span>

<span data-ttu-id="fa80b-104">Excluir uma atividade de usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fa80b-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa80b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa80b-105">Permissions</span></span>

<span data-ttu-id="fa80b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa80b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa80b-108">Permission type</span></span>      | <span data-ttu-id="fa80b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa80b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa80b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa80b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa80b-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fa80b-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fa80b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa80b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa80b-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fa80b-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fa80b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa80b-114">Application</span></span> | <span data-ttu-id="fa80b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa80b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa80b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa80b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa80b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa80b-117">Request headers</span></span>

|<span data-ttu-id="fa80b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fa80b-118">Name</span></span> | <span data-ttu-id="fa80b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa80b-119">Type</span></span> | <span data-ttu-id="fa80b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa80b-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fa80b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa80b-121">Authorization</span></span> | <span data-ttu-id="fa80b-122">string</span><span class="sxs-lookup"><span data-stu-id="fa80b-122">string</span></span> | <span data-ttu-id="fa80b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa80b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa80b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa80b-125">Request body</span></span>

<span data-ttu-id="fa80b-126">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa80b-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="fa80b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa80b-127">Response</span></span>

<span data-ttu-id="fa80b-128">Se tiver êxito, este método retornará `204 No Content` o código de resposta se a atividade tiver sido excluída.</span><span class="sxs-lookup"><span data-stu-id="fa80b-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="fa80b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa80b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa80b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa80b-130">Request</span></span>

<span data-ttu-id="fa80b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa80b-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="fa80b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa80b-132">Response</span></span>

<span data-ttu-id="fa80b-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa80b-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa80b-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fa80b-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fa80b-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa80b-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_activity-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa80b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa80b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_activity-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fa80b-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa80b-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_activity-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
