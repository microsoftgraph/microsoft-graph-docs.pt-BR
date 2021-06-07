---
title: Excluir schedulingGroup
description: Marcar um schedulingGroup como inativo definindo sua propriedade isActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 751d40329b06fe694c7bf0c53e9dc9499b5fee57
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788007"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="02139-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="02139-103">Delete schedulingGroup</span></span>

<span data-ttu-id="02139-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02139-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02139-105">Marque um [schedulingGroup](../resources/schedulinggroup.md) como inativo definindo sua **propriedade isActive.**</span><span class="sxs-lookup"><span data-stu-id="02139-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="02139-106">Este método não remove o [scheduleingGroup](../resources/schedulinggroup.md) da agenda.</span><span class="sxs-lookup"><span data-stu-id="02139-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="02139-107">As instâncias [de turno](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="02139-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="02139-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="02139-108">Permissions</span></span>

<span data-ttu-id="02139-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02139-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02139-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02139-111">Permission type</span></span>      | <span data-ttu-id="02139-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02139-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02139-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02139-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02139-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02139-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="02139-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02139-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02139-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02139-116">Not supported.</span></span>    |
|<span data-ttu-id="02139-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02139-117">Application</span></span> | <span data-ttu-id="02139-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02139-118">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02139-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02139-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="02139-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02139-120">Request headers</span></span>

| <span data-ttu-id="02139-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02139-121">Header</span></span>       | <span data-ttu-id="02139-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02139-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="02139-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02139-123">Authorization</span></span>  | <span data-ttu-id="02139-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02139-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02139-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02139-126">Request body</span></span>
<span data-ttu-id="02139-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02139-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02139-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02139-128">Response</span></span>

<span data-ttu-id="02139-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02139-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02139-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02139-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="02139-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02139-132">Request</span></span>

<span data-ttu-id="02139-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02139-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02139-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="02139-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="02139-135">C#</span><span class="sxs-lookup"><span data-stu-id="02139-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02139-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02139-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02139-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02139-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02139-138">Java</span><span class="sxs-lookup"><span data-stu-id="02139-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-delete-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02139-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02139-139">Response</span></span>

<span data-ttu-id="02139-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02139-140">The following is an example of the response.</span></span> 

><span data-ttu-id="02139-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02139-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


