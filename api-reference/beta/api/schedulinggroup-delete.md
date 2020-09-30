---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f19f6f4f228b400b66345df16fcd1320f3aa31d7
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314612"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="2fbdf-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2fbdf-103">Delete schedulingGroup</span></span>

<span data-ttu-id="2fbdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fbdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fbdf-105">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="2fbdf-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="2fbdf-106">Esse método não [Remove o enhorário do plano.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="2fbdf-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="2fbdf-107">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fbdf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fbdf-108">Permissions</span></span>

<span data-ttu-id="2fbdf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fbdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fbdf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fbdf-111">Permission type</span></span>      | <span data-ttu-id="2fbdf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fbdf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fbdf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fbdf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2fbdf-114">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2fbdf-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2fbdf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fbdf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fbdf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-116">Not supported.</span></span>    |
|<span data-ttu-id="2fbdf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fbdf-117">Application</span></span> | <span data-ttu-id="2fbdf-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fbdf-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fbdf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fbdf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="2fbdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbdf-120">Request headers</span></span>

| <span data-ttu-id="2fbdf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fbdf-121">Header</span></span>       | <span data-ttu-id="2fbdf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2fbdf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2fbdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fbdf-123">Authorization</span></span>  | <span data-ttu-id="2fbdf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2fbdf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbdf-126">Request body</span></span>
<span data-ttu-id="2fbdf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fbdf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fbdf-128">Response</span></span>

<span data-ttu-id="2fbdf-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fbdf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fbdf-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2fbdf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fbdf-132">Request</span></span>

<span data-ttu-id="2fbdf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fbdf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fbdf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="2fbdf-135">C#</span><span class="sxs-lookup"><span data-stu-id="2fbdf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fbdf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fbdf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fbdf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fbdf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fbdf-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fbdf-138">Response</span></span>

<span data-ttu-id="2fbdf-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-139">The following is an example of the response.</span></span> 

><span data-ttu-id="2fbdf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fbdf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


