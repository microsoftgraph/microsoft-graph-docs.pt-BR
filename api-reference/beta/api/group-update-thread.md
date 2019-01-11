---
title: Atualizar thread de conversas
description: Atualize um objeto thread.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a54a450064fc886e18687c31bb05ddc25868326c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878915"
---
# <a name="update-conversation-thread"></a><span data-ttu-id="8f08c-103">Atualizar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="8f08c-103">Update conversation thread</span></span>

> <span data-ttu-id="8f08c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f08c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f08c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f08c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f08c-106">Atualize um objeto [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="8f08c-106">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f08c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f08c-107">Permissions</span></span>
<span data-ttu-id="8f08c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f08c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f08c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f08c-110">Permission type</span></span>      | <span data-ttu-id="8f08c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f08c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f08c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f08c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f08c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f08c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f08c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f08c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f08c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f08c-115">Not supported.</span></span>    |
|<span data-ttu-id="8f08c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f08c-116">Application</span></span> | <span data-ttu-id="8f08c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f08c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f08c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f08c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f08c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08c-119">Request headers</span></span>
| <span data-ttu-id="8f08c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8f08c-120">Name</span></span>       | <span data-ttu-id="8f08c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f08c-121">Type</span></span> | <span data-ttu-id="8f08c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f08c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8f08c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f08c-123">Authorization</span></span>  | <span data-ttu-id="8f08c-124">string</span><span class="sxs-lookup"><span data-stu-id="8f08c-124">string</span></span>  | <span data-ttu-id="8f08c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f08c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f08c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08c-127">Request body</span></span>
<span data-ttu-id="8f08c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8f08c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="8f08c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f08c-131">Response</span></span>
<span data-ttu-id="8f08c-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f08c-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f08c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f08c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8f08c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f08c-134">Request</span></span>
<span data-ttu-id="8f08c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f08c-135">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="8f08c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f08c-136">Response</span></span>
<span data-ttu-id="8f08c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f08c-137">The following is an example of the response.</span></span>

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
