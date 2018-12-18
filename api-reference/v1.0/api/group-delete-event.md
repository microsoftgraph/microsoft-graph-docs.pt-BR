---
title: Excluir evento
description: Excluir um objeto event.
author: dkershaw10
ms.openlocfilehash: cda4cac58ef1a925aa54d63e7ba0f975a44935be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301600"
---
# <a name="delete-event"></a><span data-ttu-id="d9695-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="d9695-103">Delete event</span></span>
<span data-ttu-id="d9695-104">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d9695-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9695-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9695-105">Permissions</span></span>
<span data-ttu-id="d9695-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9695-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9695-108">Permission type</span></span>      | <span data-ttu-id="d9695-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9695-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9695-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9695-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9695-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9695-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9695-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9695-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9695-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9695-113">Not supported.</span></span>    |
|<span data-ttu-id="d9695-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9695-114">Application</span></span> | <span data-ttu-id="d9695-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9695-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9695-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9695-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d9695-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9695-117">Request headers</span></span>
| <span data-ttu-id="d9695-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d9695-118">Name</span></span>       | <span data-ttu-id="d9695-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9695-119">Type</span></span> | <span data-ttu-id="d9695-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9695-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9695-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9695-121">Authorization</span></span>  | <span data-ttu-id="d9695-122">string</span><span class="sxs-lookup"><span data-stu-id="d9695-122">string</span></span>  | <span data-ttu-id="d9695-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9695-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9695-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9695-125">Request body</span></span>
<span data-ttu-id="d9695-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9695-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9695-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9695-127">Response</span></span>
<span data-ttu-id="d9695-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9695-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9695-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9695-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d9695-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9695-131">Request</span></span>
<span data-ttu-id="d9695-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9695-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="d9695-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9695-133">Response</span></span>
<span data-ttu-id="d9695-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9695-134">The following is an example of the response.</span></span> 
><span data-ttu-id="d9695-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9695-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->