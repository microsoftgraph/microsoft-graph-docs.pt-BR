---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a23472db0b87204ed3dd3e7408154738a940103
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867901"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="51a06-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="51a06-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51a06-104">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="51a06-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="51a06-105">Esse método não [Remove o enhorário do plano.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="51a06-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="51a06-106">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="51a06-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="51a06-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="51a06-107">Permissions</span></span>

<span data-ttu-id="51a06-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51a06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51a06-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51a06-110">Permission type</span></span>      | <span data-ttu-id="51a06-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51a06-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51a06-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51a06-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51a06-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51a06-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="51a06-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51a06-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51a06-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51a06-115">Not supported.</span></span>    |
|<span data-ttu-id="51a06-116">Application</span><span class="sxs-lookup"><span data-stu-id="51a06-116">Application</span></span> | <span data-ttu-id="51a06-117">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="51a06-117">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="51a06-118">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="51a06-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="51a06-119">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="51a06-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="51a06-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="51a06-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="51a06-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51a06-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="51a06-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51a06-122">Request headers</span></span>

| <span data-ttu-id="51a06-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51a06-123">Header</span></span>       | <span data-ttu-id="51a06-124">Valor</span><span class="sxs-lookup"><span data-stu-id="51a06-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="51a06-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="51a06-125">Authorization</span></span>  | <span data-ttu-id="51a06-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51a06-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51a06-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51a06-128">Request body</span></span>
<span data-ttu-id="51a06-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51a06-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51a06-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a06-130">Response</span></span>

<span data-ttu-id="51a06-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51a06-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51a06-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51a06-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="51a06-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51a06-134">Request</span></span>

<span data-ttu-id="51a06-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51a06-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51a06-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="51a06-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51a06-137">C#</span><span class="sxs-lookup"><span data-stu-id="51a06-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51a06-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51a06-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51a06-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51a06-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51a06-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="51a06-140">Response</span></span>

<span data-ttu-id="51a06-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51a06-141">The following is an example of the response.</span></span> 

><span data-ttu-id="51a06-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51a06-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
