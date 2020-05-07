---
title: Excluir schedulingGroup
description: Marcar um modo de agendamento como inativo Configurando sua propriedade IsActive
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7aae33e48ca3170cdc2ce06e96d704139ec13f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155135"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="8654b-103">Excluir schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="8654b-103">Delete schedulingGroup</span></span>

<span data-ttu-id="8654b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8654b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8654b-105">Marcar um modo de [agendamento](../resources/schedulinggroup.md) como inativo, definindo sua propriedade **IsActive** .</span><span class="sxs-lookup"><span data-stu-id="8654b-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="8654b-106">Esse método não [Remove o enhorário do plano.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="8654b-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="8654b-107">As instâncias de [alternância](../resources/shift.md) existentes atribuídas ao grupo de agendamento permanecem como parte do grupo.</span><span class="sxs-lookup"><span data-stu-id="8654b-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8654b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8654b-108">Permissions</span></span>

<span data-ttu-id="8654b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8654b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8654b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8654b-111">Permission type</span></span>      | <span data-ttu-id="8654b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8654b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8654b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8654b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8654b-114">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8654b-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8654b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8654b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8654b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8654b-116">Not supported.</span></span>    |
|<span data-ttu-id="8654b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8654b-117">Application</span></span> | <span data-ttu-id="8654b-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8654b-118">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="8654b-119">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="8654b-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8654b-120">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="8654b-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8654b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8654b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="8654b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8654b-122">Request headers</span></span>

| <span data-ttu-id="8654b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8654b-123">Header</span></span>       | <span data-ttu-id="8654b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8654b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8654b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8654b-125">Authorization</span></span>  | <span data-ttu-id="8654b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8654b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8654b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8654b-128">Request body</span></span>
<span data-ttu-id="8654b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8654b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8654b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8654b-130">Response</span></span>

<span data-ttu-id="8654b-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8654b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8654b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8654b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8654b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8654b-134">Request</span></span>

<span data-ttu-id="8654b-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8654b-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="8654b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8654b-136">Response</span></span>

<span data-ttu-id="8654b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8654b-137">The following is an example of the response.</span></span> 

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
