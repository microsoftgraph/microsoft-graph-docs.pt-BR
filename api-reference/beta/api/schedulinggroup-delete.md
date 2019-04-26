---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6a41108349d7e398d10afd183273f731cf947fe8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331369"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="fad91-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="fad91-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fad91-104">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade IsActive. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="fad91-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="fad91-105">Esse método não remove o enhorário do plano. [](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="fad91-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="fad91-106">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="fad91-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="fad91-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fad91-107">Permissions</span></span>

<span data-ttu-id="fad91-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fad91-110">Permission type</span></span>      | <span data-ttu-id="fad91-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fad91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fad91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fad91-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fad91-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad91-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fad91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fad91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fad91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fad91-115">Not supported.</span></span>    |
|<span data-ttu-id="fad91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fad91-116">Application</span></span> | <span data-ttu-id="fad91-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fad91-117">Not supported.</span></span> |

> <span data-ttu-id="fad91-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fad91-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fad91-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="fad91-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fad91-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fad91-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="fad91-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fad91-121">Request headers</span></span>

| <span data-ttu-id="fad91-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fad91-122">Header</span></span>       | <span data-ttu-id="fad91-123">Valor</span><span class="sxs-lookup"><span data-stu-id="fad91-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fad91-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fad91-124">Authorization</span></span>  | <span data-ttu-id="fad91-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fad91-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fad91-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fad91-127">Content-Type</span></span>  | <span data-ttu-id="fad91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fad91-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fad91-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fad91-129">Request body</span></span>
<span data-ttu-id="fad91-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fad91-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fad91-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad91-131">Response</span></span>

<span data-ttu-id="fad91-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fad91-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad91-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fad91-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fad91-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fad91-135">Request</span></span>

<span data-ttu-id="fad91-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fad91-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="fad91-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad91-137">Response</span></span>

<span data-ttu-id="fad91-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fad91-138">The following is an example of the response.</span></span> 

><span data-ttu-id="fad91-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fad91-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
