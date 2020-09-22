---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9c5eabe4503bf8ac3f6d98d16a0a85a6f01d5af4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071924"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="aa433-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="aa433-103">Delete schedulingGroup</span></span>

<span data-ttu-id="aa433-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa433-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa433-105">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="aa433-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="aa433-106">Esse método não [Remove o enhorário do plano.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="aa433-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="aa433-107">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="aa433-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa433-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa433-108">Permissions</span></span>

<span data-ttu-id="aa433-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa433-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa433-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa433-111">Permission type</span></span>      | <span data-ttu-id="aa433-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa433-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa433-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa433-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa433-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa433-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aa433-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa433-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa433-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa433-116">Not supported.</span></span>    |
|<span data-ttu-id="aa433-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa433-117">Application</span></span> | <span data-ttu-id="aa433-118">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="aa433-118">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="aa433-119">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="aa433-119">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="aa433-120">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="aa433-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aa433-121">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="aa433-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa433-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa433-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="aa433-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa433-123">Request headers</span></span>

| <span data-ttu-id="aa433-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa433-124">Header</span></span>       | <span data-ttu-id="aa433-125">Valor</span><span class="sxs-lookup"><span data-stu-id="aa433-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aa433-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa433-126">Authorization</span></span>  | <span data-ttu-id="aa433-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa433-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa433-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa433-129">Request body</span></span>
<span data-ttu-id="aa433-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa433-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa433-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa433-131">Response</span></span>

<span data-ttu-id="aa433-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa433-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa433-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa433-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aa433-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa433-135">Request</span></span>

<span data-ttu-id="aa433-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa433-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa433-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa433-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="aa433-138">C#</span><span class="sxs-lookup"><span data-stu-id="aa433-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa433-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa433-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa433-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa433-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aa433-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa433-141">Response</span></span>

<span data-ttu-id="aa433-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa433-142">The following is an example of the response.</span></span> 

><span data-ttu-id="aa433-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa433-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


