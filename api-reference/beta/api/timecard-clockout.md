---
title: 'timeCard: clockOut'
description: Clock Out para finalizar um cartão de ponto aberto.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6130fd23ee476c66bdda77140834d8ce484cc80d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787843"
---
# <a name="timecard-clockout"></a><span data-ttu-id="58876-103">timeCard: clockOut</span><span class="sxs-lookup"><span data-stu-id="58876-103">timeCard: clockOut</span></span>

<span data-ttu-id="58876-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58876-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58876-105">Clock out to end a open [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="58876-105">Clock out to end an open [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58876-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="58876-106">Permissions</span></span>

<span data-ttu-id="58876-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58876-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58876-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58876-109">Permission type</span></span>      | <span data-ttu-id="58876-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58876-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58876-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58876-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58876-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58876-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="58876-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58876-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58876-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58876-114">Not supported.</span></span>    |
|<span data-ttu-id="58876-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58876-115">Application</span></span> | <span data-ttu-id="58876-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="58876-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="58876-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="58876-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="58876-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58876-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/clockOut
```

## <a name="request-headers"></a><span data-ttu-id="58876-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58876-119">Request headers</span></span>

| <span data-ttu-id="58876-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58876-120">Header</span></span>       | <span data-ttu-id="58876-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58876-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="58876-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58876-122">Authorization</span></span>  | <span data-ttu-id="58876-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58876-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="58876-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="58876-125">Content-type</span></span> | <span data-ttu-id="58876-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58876-p103">application/json. Required.</span></span>|
| <span data-ttu-id="58876-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="58876-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="58876-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="58876-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="58876-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58876-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58876-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58876-131">Request body</span></span>

<span data-ttu-id="58876-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58876-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58876-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58876-133">Parameter</span></span>    | <span data-ttu-id="58876-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="58876-134">Type</span></span>        | <span data-ttu-id="58876-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="58876-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58876-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="58876-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="58876-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="58876-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="58876-138">notes</span><span class="sxs-lookup"><span data-stu-id="58876-138">notes</span></span>| [<span data-ttu-id="58876-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="58876-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="58876-140">Observações para o tempo de saída.</span><span class="sxs-lookup"><span data-stu-id="58876-140">Notes for the clock out.</span></span> |

## <a name="response"></a><span data-ttu-id="58876-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="58876-141">Response</span></span>

<span data-ttu-id="58876-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="58876-142">If successful, this method returns a `204 No Content` response code.</span></span>


## <a name="example"></a><span data-ttu-id="58876-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58876-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="58876-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58876-144">Request</span></span>
<span data-ttu-id="58876-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58876-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-clockout"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/clockout
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock out smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="58876-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="58876-146">Response</span></span>

<span data-ttu-id="58876-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58876-147">The following is an example of the response.</span></span> 

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
  "description": "Clock Out",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
