---
title: 'agendamento: share'
description: Compartilhar um intervalo de tempo de agendamento com membros de agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fce02b8f18a2745b06d1782ecadb7bc7bd3adc0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154238"
---
# <a name="schedule-share"></a><span data-ttu-id="98174-103">agendamento: share</span><span class="sxs-lookup"><span data-stu-id="98174-103">schedule: share</span></span>

<span data-ttu-id="98174-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98174-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98174-105">Compartilhar um intervalo de tempo de [agendamento](../resources/schedule.md) com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="98174-105">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="98174-106">Faça as coleções de itens [Shift](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado da [agenda](../resources/schedule.md) exibida pelos membros da equipe especificados, incluindo funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="98174-106">Make the collections of [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="98174-107">Cada [mudança](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) instância em um [cronograma](../resources/schedule.md) suporta uma versão de rascunho e uma versão compartilhada do item.</span><span class="sxs-lookup"><span data-stu-id="98174-107">Each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="98174-108">A versão de rascunho é visível apenas por gerentes e a versão compartilhada é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="98174-108">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="98174-109">Para cada [mudança](../resources/shift.md), [openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) instância no intervalo de tempo especificado, a ação de compartilhamento atualiza a versão compartilhada da versão de rascunho, para que, além dos gerentes, os funcionários também possam exibir as informações mais recentes sobre o item.</span><span class="sxs-lookup"><span data-stu-id="98174-109">For each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="98174-110">O parâmetro **notifyTeam** especifica ainda mais quais funcionários podem exibir o item.</span><span class="sxs-lookup"><span data-stu-id="98174-110">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="98174-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="98174-111">Permissions</span></span>

<span data-ttu-id="98174-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98174-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98174-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98174-114">Permission type</span></span>      | <span data-ttu-id="98174-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="98174-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98174-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98174-116">Delegated (work or school account)</span></span> | <span data-ttu-id="98174-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98174-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98174-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98174-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98174-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98174-119">Not supported.</span></span>    |
|<span data-ttu-id="98174-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98174-120">Application</span></span> | <span data-ttu-id="98174-121">Schedule. ReadWrite. All \*</span><span class="sxs-lookup"><span data-stu-id="98174-121">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="98174-122">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="98174-122">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="98174-123">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="98174-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="98174-124">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="98174-124">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="98174-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98174-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="98174-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98174-126">Request headers</span></span>

| <span data-ttu-id="98174-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98174-127">Header</span></span>       | <span data-ttu-id="98174-128">Valor</span><span class="sxs-lookup"><span data-stu-id="98174-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98174-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="98174-129">Authorization</span></span>  | <span data-ttu-id="98174-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98174-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="98174-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="98174-132">Content-Type</span></span>  | <span data-ttu-id="98174-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98174-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98174-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98174-135">Request body</span></span>

<span data-ttu-id="98174-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98174-136">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="98174-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="98174-137">Parameter</span></span>                   |<span data-ttu-id="98174-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="98174-138">Type</span></span>           |<span data-ttu-id="98174-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="98174-139">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="98174-140">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="98174-140">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="98174-141">Indica se a equipe inteira deve receber uma notificação visível desta ação ou apenas os funcionários que têm uma alteração atribuída a elas que foram compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="98174-141">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="98174-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98174-142">Required.</span></span>       |
| <span data-ttu-id="98174-143">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98174-143">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="98174-144">O horário de início para compartilhar as mudanças no cronograma.</span><span class="sxs-lookup"><span data-stu-id="98174-144">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="98174-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98174-145">Required.</span></span>   |
| <span data-ttu-id="98174-146">endDateTime</span><span class="sxs-lookup"><span data-stu-id="98174-146">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="98174-147">O horário de término para compartilhar turnos no cronograma até.</span><span class="sxs-lookup"><span data-stu-id="98174-147">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="98174-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="98174-148">Response</span></span>

<span data-ttu-id="98174-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98174-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98174-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98174-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="98174-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98174-152">Request</span></span>

<span data-ttu-id="98174-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="98174-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98174-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="98174-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="98174-155">C#</span><span class="sxs-lookup"><span data-stu-id="98174-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98174-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98174-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98174-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98174-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="98174-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="98174-158">Response</span></span>

<span data-ttu-id="98174-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="98174-159">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
