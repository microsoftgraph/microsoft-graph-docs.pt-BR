---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1a9637876071c499ce8cfd9da40d211c4b4f91c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015586"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="bc8db-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="bc8db-103">Delete schedulingGroup</span></span>

<span data-ttu-id="bc8db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc8db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc8db-105">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="bc8db-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="bc8db-106">Esse método não [Remove o enhorário do plano.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="bc8db-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="bc8db-107">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="bc8db-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc8db-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc8db-108">Permissions</span></span>

<span data-ttu-id="bc8db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc8db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc8db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc8db-111">Permission type</span></span>      | <span data-ttu-id="bc8db-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc8db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc8db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc8db-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc8db-114">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bc8db-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc8db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc8db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc8db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc8db-116">Not supported.</span></span>    |
|<span data-ttu-id="bc8db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc8db-117">Application</span></span> | <span data-ttu-id="bc8db-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc8db-118">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="bc8db-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="bc8db-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bc8db-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="bc8db-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bc8db-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc8db-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="bc8db-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8db-122">Request headers</span></span>

| <span data-ttu-id="bc8db-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc8db-123">Header</span></span>       | <span data-ttu-id="bc8db-124">Valor</span><span class="sxs-lookup"><span data-stu-id="bc8db-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc8db-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc8db-125">Authorization</span></span>  | <span data-ttu-id="bc8db-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc8db-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc8db-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8db-128">Request body</span></span>
<span data-ttu-id="bc8db-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc8db-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc8db-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8db-130">Response</span></span>

<span data-ttu-id="bc8db-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc8db-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc8db-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc8db-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc8db-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc8db-134">Request</span></span>

<span data-ttu-id="bc8db-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc8db-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bc8db-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc8db-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="bc8db-137">C#</span><span class="sxs-lookup"><span data-stu-id="bc8db-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc8db-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc8db-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc8db-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc8db-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc8db-140">Java</span><span class="sxs-lookup"><span data-stu-id="bc8db-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="bc8db-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc8db-141">Response</span></span>

<span data-ttu-id="bc8db-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc8db-142">The following is an example of the response.</span></span> 

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

