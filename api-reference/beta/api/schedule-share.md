---
title: 'agendamento: share'
description: Compartilhar um intervalo de tempo de agendamento com membros de agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a1e86d397b871ed78f867695e272368b2bcb5eb4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638946"
---
# <a name="schedule-share"></a><span data-ttu-id="59def-103">agendamento: share</span><span class="sxs-lookup"><span data-stu-id="59def-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59def-104">Compartilhar um intervalo de tempo de [agendamento](../resources/schedule.md) com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="59def-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="59def-105">Faça as coleções de itens [Shift](../resources/shift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado da [agenda](../resources/schedule.md) exibida pelos membros da equipe especificados, incluindo funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="59def-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="59def-106">Cada [mudança](../resources/shift.md) e [timeOff](../resources/timeoff.md) instância em um [cronograma](../resources/schedule.md) oferece suporte a uma versão de rascunho e uma versão compartilhada do item.</span><span class="sxs-lookup"><span data-stu-id="59def-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="59def-107">A versão de rascunho é visível apenas por gerentes e a versão compartilhada é visível por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="59def-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="59def-108">Para cada [mudança](../resources/shift.md) e [timeOff](../resources/timeoff.md) instância no intervalo de tempo especificado, a ação de compartilhamento atualiza a versão compartilhada da versão de rascunho, para que, além dos gerentes, os funcionários também possam exibir as informações mais atuais sobre o item.</span><span class="sxs-lookup"><span data-stu-id="59def-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="59def-109">O parâmetro **notifyTeam** especifica ainda mais quais funcionários podem exibir o item.</span><span class="sxs-lookup"><span data-stu-id="59def-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="59def-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="59def-110">Permissions</span></span>

<span data-ttu-id="59def-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59def-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59def-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59def-113">Permission type</span></span>      | <span data-ttu-id="59def-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59def-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59def-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59def-115">Delegated (work or school account)</span></span> | <span data-ttu-id="59def-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59def-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59def-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59def-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59def-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59def-118">Not supported.</span></span>    |
|<span data-ttu-id="59def-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59def-119">Application</span></span> | <span data-ttu-id="59def-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59def-120">Not supported.</span></span> |

> <span data-ttu-id="59def-121">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="59def-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="59def-122">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="59def-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="59def-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59def-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="59def-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59def-124">Request headers</span></span>

| <span data-ttu-id="59def-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59def-125">Header</span></span>       | <span data-ttu-id="59def-126">Valor</span><span class="sxs-lookup"><span data-stu-id="59def-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59def-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="59def-127">Authorization</span></span>  | <span data-ttu-id="59def-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59def-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59def-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59def-130">Content-Type</span></span>  | <span data-ttu-id="59def-131">application/json</span><span class="sxs-lookup"><span data-stu-id="59def-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59def-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59def-132">Request body</span></span>

<span data-ttu-id="59def-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59def-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="59def-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59def-134">Parameter</span></span>                   |<span data-ttu-id="59def-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="59def-135">Type</span></span>           |<span data-ttu-id="59def-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="59def-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="59def-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="59def-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="59def-138">Indica se a equipe inteira deve receber uma notificação visível desta ação ou apenas os funcionários que têm uma alteração atribuída a elas que foram compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="59def-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="59def-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59def-139">Required.</span></span>       |
| <span data-ttu-id="59def-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59def-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="59def-141">O horário de início para compartilhar as mudanças no cronograma.</span><span class="sxs-lookup"><span data-stu-id="59def-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="59def-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59def-142">Required.</span></span>   |
| <span data-ttu-id="59def-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59def-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="59def-144">O horário de término para compartilhar turnos no cronograma até.</span><span class="sxs-lookup"><span data-stu-id="59def-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="59def-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="59def-145">Response</span></span>

<span data-ttu-id="59def-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59def-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59def-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59def-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59def-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59def-149">Request</span></span>

<span data-ttu-id="59def-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59def-150">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="59def-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="59def-151">Response</span></span>

<span data-ttu-id="59def-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59def-152">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="59def-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="59def-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="59def-154">Basic</span><span class="sxs-lookup"><span data-stu-id="59def-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-share-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59def-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59def-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-share-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
