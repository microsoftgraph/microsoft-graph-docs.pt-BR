---
title: Excluir evento
description: Excluir um objeto event.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c42fa9942e25150c9cba7e5e2557ae35353c2d76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524062"
---
# <a name="delete-event"></a><span data-ttu-id="008c2-103">Excluir evento</span><span class="sxs-lookup"><span data-stu-id="008c2-103">Delete event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="008c2-104">Excluir um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="008c2-104">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="008c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="008c2-105">Permissions</span></span>
<span data-ttu-id="008c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="008c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="008c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="008c2-108">Permission type</span></span>      | <span data-ttu-id="008c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="008c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="008c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="008c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="008c2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="008c2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="008c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="008c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="008c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="008c2-113">Not supported.</span></span>    |
|<span data-ttu-id="008c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="008c2-114">Application</span></span> | <span data-ttu-id="008c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="008c2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="008c2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="008c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="008c2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="008c2-117">Request headers</span></span>
| <span data-ttu-id="008c2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="008c2-118">Name</span></span>       | <span data-ttu-id="008c2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="008c2-119">Type</span></span> | <span data-ttu-id="008c2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="008c2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="008c2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="008c2-121">Authorization</span></span>  | <span data-ttu-id="008c2-122">string</span><span class="sxs-lookup"><span data-stu-id="008c2-122">string</span></span>  | <span data-ttu-id="008c2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="008c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="008c2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="008c2-125">Request body</span></span>
<span data-ttu-id="008c2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="008c2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="008c2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="008c2-127">Response</span></span>
<span data-ttu-id="008c2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="008c2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="008c2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="008c2-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="008c2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="008c2-131">Request</span></span>
<span data-ttu-id="008c2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="008c2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="008c2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="008c2-133">Response</span></span>
<span data-ttu-id="008c2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="008c2-134">The following is an example of the response.</span></span> 
><span data-ttu-id="008c2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="008c2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-event.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
