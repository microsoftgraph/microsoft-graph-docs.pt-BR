---
title: Atualizar thread de conversas
description: Atualize um objeto thread.
ms.openlocfilehash: 56492be24d0e917bfed1cbe8f066f16bac873d14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039289"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="8df22-103">Atualizar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="8df22-103">Update conversation thread</span></span>

> <span data-ttu-id="8df22-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8df22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8df22-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8df22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8df22-106">Atualize um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="8df22-106">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8df22-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8df22-107">Permissions</span></span>
<span data-ttu-id="8df22-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8df22-110">Permission type</span></span>      | <span data-ttu-id="8df22-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8df22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8df22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8df22-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8df22-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df22-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8df22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8df22-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8df22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df22-115">Not supported.</span></span>    |
|<span data-ttu-id="8df22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8df22-116">Application</span></span> | <span data-ttu-id="8df22-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8df22-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8df22-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8df22-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8df22-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8df22-119">Request headers</span></span>
| <span data-ttu-id="8df22-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8df22-120">Name</span></span>       | <span data-ttu-id="8df22-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8df22-121">Type</span></span> | <span data-ttu-id="8df22-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df22-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8df22-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8df22-123">Authorization</span></span>  | <span data-ttu-id="8df22-124">string</span><span class="sxs-lookup"><span data-stu-id="8df22-124">string</span></span>  | <span data-ttu-id="8df22-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8df22-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8df22-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8df22-127">Request body</span></span>
<span data-ttu-id="8df22-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8df22-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="8df22-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df22-131">Response</span></span>
<span data-ttu-id="8df22-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8df22-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8df22-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8df22-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8df22-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8df22-134">Request</span></span>
<span data-ttu-id="8df22-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8df22-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="8df22-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8df22-136">Response</span></span>
<span data-ttu-id="8df22-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8df22-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->