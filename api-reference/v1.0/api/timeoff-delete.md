---
title: Excluir timeOff
description: Excluir uma instância do timeOff de um agendamento.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28943ba690dfb59385a81edd38f2d54d4746a5a5
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155030"
---
# <a name="delete-timeoff"></a><span data-ttu-id="c3eaf-103">Excluir timeOff</span><span class="sxs-lookup"><span data-stu-id="c3eaf-103">Delete timeOff</span></span>

<span data-ttu-id="c3eaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3eaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3eaf-105">Excluir uma instância do [timeOff](../resources/timeoff.md) de um [agendamento](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="c3eaf-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3eaf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3eaf-106">Permissions</span></span>

<span data-ttu-id="c3eaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3eaf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3eaf-109">Permission type</span></span>      | <span data-ttu-id="c3eaf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3eaf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3eaf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3eaf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3eaf-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3eaf-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3eaf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3eaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3eaf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-114">Not supported.</span></span>    |
|<span data-ttu-id="c3eaf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3eaf-115">Application</span></span> | <span data-ttu-id="c3eaf-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3eaf-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="c3eaf-117">**Observação**: esta API oferece suporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c3eaf-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c3eaf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3eaf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="c3eaf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3eaf-120">Request headers</span></span>

| <span data-ttu-id="c3eaf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3eaf-121">Header</span></span>       | <span data-ttu-id="c3eaf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c3eaf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3eaf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3eaf-123">Authorization</span></span>  | <span data-ttu-id="c3eaf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3eaf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3eaf-126">Request body</span></span>
<span data-ttu-id="c3eaf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3eaf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3eaf-128">Response</span></span>

<span data-ttu-id="c3eaf-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3eaf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3eaf-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3eaf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3eaf-132">Request</span></span>

<span data-ttu-id="c3eaf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```

---


#### <a name="response"></a><span data-ttu-id="c3eaf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3eaf-134">Response</span></span>

<span data-ttu-id="c3eaf-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c3eaf-135">The following is an example of the response.</span></span> 

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
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
