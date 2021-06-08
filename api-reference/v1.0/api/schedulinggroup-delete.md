---
title: Excluir schedulingGroup
description: Marcar um schedulingGroup como inativo definindo sua propriedade isActive
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09d54084537636fb41aff7f5557b05e0d6d8fbe7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786305"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="2495e-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="2495e-103">Delete schedulingGroup</span></span>

<span data-ttu-id="2495e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2495e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2495e-105">Marque um [schedulingGroup](../resources/schedulinggroup.md) como inativo definindo sua **propriedade isActive.**</span><span class="sxs-lookup"><span data-stu-id="2495e-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="2495e-106">Este método não remove o [scheduleingGroup](../resources/schedulinggroup.md) da agenda.</span><span class="sxs-lookup"><span data-stu-id="2495e-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="2495e-107">As instâncias [de turno](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="2495e-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2495e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2495e-108">Permissions</span></span>

<span data-ttu-id="2495e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2495e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2495e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2495e-111">Permission type</span></span>      | <span data-ttu-id="2495e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2495e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2495e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2495e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2495e-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2495e-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2495e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2495e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2495e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2495e-116">Not supported.</span></span>    |
|<span data-ttu-id="2495e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2495e-117">Application</span></span> | <span data-ttu-id="2495e-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2495e-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2495e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2495e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="2495e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2495e-120">Request headers</span></span>

| <span data-ttu-id="2495e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2495e-121">Header</span></span>       | <span data-ttu-id="2495e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2495e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2495e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2495e-123">Authorization</span></span>  | <span data-ttu-id="2495e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2495e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2495e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2495e-126">Request body</span></span>
<span data-ttu-id="2495e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2495e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2495e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2495e-128">Response</span></span>

<span data-ttu-id="2495e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2495e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2495e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2495e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2495e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2495e-132">Request</span></span>

<span data-ttu-id="2495e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2495e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2495e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2495e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="2495e-135">C#</span><span class="sxs-lookup"><span data-stu-id="2495e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2495e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2495e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2495e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2495e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2495e-138">Java</span><span class="sxs-lookup"><span data-stu-id="2495e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="2495e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2495e-139">Response</span></span>

<span data-ttu-id="2495e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2495e-140">The following is an example of the response.</span></span> 

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
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

