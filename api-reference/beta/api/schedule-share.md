---
title: 'schedule: share'
description: Compartilhe um intervalo de tempo de agendamento com membros de agendamento.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 47bd1e71b31a10b7dfb0ffc34c063d94f2e065fc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788014"
---
# <a name="schedule-share"></a><span data-ttu-id="59446-103">schedule: share</span><span class="sxs-lookup"><span data-stu-id="59446-103">schedule: share</span></span>

<span data-ttu-id="59446-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59446-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59446-105">Compartilhe um [intervalo de](../resources/schedule.md) tempo de agendamento com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="59446-105">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="59446-106">Tornar as coleções de itens [shift](../resources/shift.md), [openshift](../resources/openshift.md) e [](../resources/schedule.md) [timeOff](../resources/timeoff.md) no intervalo de tempo especificado do cronograma visualizado pelos membros da equipe especificados, incluindo funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="59446-106">Make the collections of [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="59446-107">Cada [turno](../resources/shift.md), [instância openshift](../resources/openshift.md) [](../resources/schedule.md) [e timeOff](../resources/timeoff.md) em uma agenda suporta uma versão de rascunho e uma versão compartilhada do item.</span><span class="sxs-lookup"><span data-stu-id="59446-107">Each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="59446-108">A versão de rascunho pode ser visualizada somente por gerentes, e a versão compartilhada pode ser visualizada por funcionários e gerentes.</span><span class="sxs-lookup"><span data-stu-id="59446-108">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="59446-109">Para cada [turno](../resources/shift.md), [instância openshift](../resources/openshift.md) e [timeOff](../resources/timeoff.md) no intervalo de tempo especificado, a ação de compartilhamento atualiza a versão compartilhada da versão de rascunho, para que, além dos gerentes, os funcionários também possam exibir as informações mais atuais sobre o item.</span><span class="sxs-lookup"><span data-stu-id="59446-109">For each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="59446-110">O **parâmetro notifyTeam** especifica ainda quais funcionários podem exibir o item.</span><span class="sxs-lookup"><span data-stu-id="59446-110">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="59446-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="59446-111">Permissions</span></span>

<span data-ttu-id="59446-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59446-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59446-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59446-114">Permission type</span></span>      | <span data-ttu-id="59446-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59446-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59446-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59446-116">Delegated (work or school account)</span></span> | <span data-ttu-id="59446-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59446-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="59446-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59446-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59446-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59446-119">Not supported.</span></span>    |
|<span data-ttu-id="59446-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59446-120">Application</span></span> | <span data-ttu-id="59446-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59446-121">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59446-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59446-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="59446-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59446-123">Request headers</span></span>

| <span data-ttu-id="59446-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59446-124">Header</span></span>       | <span data-ttu-id="59446-125">Valor</span><span class="sxs-lookup"><span data-stu-id="59446-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59446-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="59446-126">Authorization</span></span>  | <span data-ttu-id="59446-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59446-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59446-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59446-129">Content-Type</span></span>  | <span data-ttu-id="59446-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59446-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59446-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59446-132">Request body</span></span>

<span data-ttu-id="59446-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59446-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="59446-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59446-134">Parameter</span></span>                   |<span data-ttu-id="59446-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="59446-135">Type</span></span>           |<span data-ttu-id="59446-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="59446-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="59446-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="59446-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="59446-138">Indica se toda a equipe deve receber uma notificação visível dessa ação ou apenas os funcionários que têm um turno atribuído a eles que foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="59446-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="59446-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59446-139">Required.</span></span>       |
| <span data-ttu-id="59446-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59446-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="59446-141">A hora de início para compartilhar turnos no agendamento de.</span><span class="sxs-lookup"><span data-stu-id="59446-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="59446-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59446-142">Required.</span></span>   |
| <span data-ttu-id="59446-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="59446-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="59446-144">A hora de término para compartilhar turnos na agenda até.</span><span class="sxs-lookup"><span data-stu-id="59446-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="59446-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="59446-145">Response</span></span>

<span data-ttu-id="59446-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59446-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59446-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59446-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59446-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59446-149">Request</span></span>

<span data-ttu-id="59446-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59446-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59446-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="59446-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59446-152">C#</span><span class="sxs-lookup"><span data-stu-id="59446-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59446-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59446-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59446-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59446-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59446-155">Java</span><span class="sxs-lookup"><span data-stu-id="59446-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="59446-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="59446-156">Response</span></span>

<span data-ttu-id="59446-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59446-157">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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


