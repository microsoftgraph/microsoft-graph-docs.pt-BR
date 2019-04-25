---
title: Excluir um historyItem
description: Excluir um item de histórico existente para uma atividade existente do usuário.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 4814987367b7b9a278c645dbdca8fb5e795ce784
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576266"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="a9089-103">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="a9089-103">Delete a historyItem</span></span>

<span data-ttu-id="a9089-104">Excluir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9089-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9089-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9089-105">Permissions</span></span>

<span data-ttu-id="a9089-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9089-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a9089-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9089-108">Permission type</span></span>      | <span data-ttu-id="a9089-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9089-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9089-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9089-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9089-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a9089-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a9089-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9089-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9089-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a9089-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="a9089-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9089-114">Application</span></span> | <span data-ttu-id="a9089-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9089-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9089-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9089-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9089-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9089-117">Request headers</span></span>

|<span data-ttu-id="a9089-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a9089-118">Name</span></span> | <span data-ttu-id="a9089-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9089-119">Type</span></span> | <span data-ttu-id="a9089-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9089-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a9089-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9089-121">Authorization</span></span> | <span data-ttu-id="a9089-122">string</span><span class="sxs-lookup"><span data-stu-id="a9089-122">string</span></span> | <span data-ttu-id="a9089-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9089-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9089-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9089-125">Request body</span></span>

<span data-ttu-id="a9089-126">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9089-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="a9089-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9089-127">Response</span></span>

<span data-ttu-id="a9089-128">Se tiver êxito, este método retornará `204 No Content` o código de resposta se o item do histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="a9089-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="a9089-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9089-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a9089-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9089-130">Request</span></span>

<span data-ttu-id="a9089-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9089-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="a9089-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9089-132">Response</span></span>

<span data-ttu-id="a9089-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9089-133">Here is an example of the response.</span></span>

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
