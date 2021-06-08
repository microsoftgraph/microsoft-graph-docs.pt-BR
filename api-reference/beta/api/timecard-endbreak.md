---
title: 'timeCard: endBreak'
description: Termine a quebra aberta em um cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f88697261aae32e978e4910c8d112d55c7ceb5ab
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787838"
---
# <a name="timecard-endbreak"></a><span data-ttu-id="bdca0-103">timeCard: endBreak</span><span class="sxs-lookup"><span data-stu-id="bdca0-103">timeCard: endBreak</span></span>

<span data-ttu-id="bdca0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdca0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdca0-105">Termine a quebra aberta em um [cartão de ponto específico.](../resources/timeCard.md)</span><span class="sxs-lookup"><span data-stu-id="bdca0-105">End the open break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdca0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bdca0-106">Permissions</span></span>

<span data-ttu-id="bdca0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdca0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdca0-109">Permission type</span></span>      | <span data-ttu-id="bdca0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdca0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdca0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdca0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bdca0-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdca0-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdca0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdca0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdca0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdca0-114">Not supported.</span></span>    |
|<span data-ttu-id="bdca0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdca0-115">Application</span></span> | <span data-ttu-id="bdca0-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="bdca0-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="bdca0-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdca0-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="bdca0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdca0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/endBreak
```

## <a name="request-headers"></a><span data-ttu-id="bdca0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdca0-119">Request headers</span></span>

| <span data-ttu-id="bdca0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdca0-120">Header</span></span>       | <span data-ttu-id="bdca0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bdca0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bdca0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdca0-122">Authorization</span></span>  | <span data-ttu-id="bdca0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdca0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bdca0-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="bdca0-125">Content-type</span></span> | <span data-ttu-id="bdca0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdca0-p103">application/json. Required.</span></span>|
| <span data-ttu-id="bdca0-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="bdca0-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="bdca0-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="bdca0-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="bdca0-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdca0-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdca0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdca0-131">Request body</span></span>

<span data-ttu-id="bdca0-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdca0-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bdca0-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdca0-133">Parameter</span></span>    | <span data-ttu-id="bdca0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdca0-134">Type</span></span>        | <span data-ttu-id="bdca0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdca0-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bdca0-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="bdca0-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="bdca0-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="bdca0-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="bdca0-138">notes</span><span class="sxs-lookup"><span data-stu-id="bdca0-138">notes</span></span>| [<span data-ttu-id="bdca0-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="bdca0-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="bdca0-140">Observações durante o término do intervalo.</span><span class="sxs-lookup"><span data-stu-id="bdca0-140">Notes during end of break.</span></span>|

## <a name="response"></a><span data-ttu-id="bdca0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdca0-141">Response</span></span>

<span data-ttu-id="bdca0-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bdca0-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bdca0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdca0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdca0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdca0-144">Request</span></span>
<span data-ttu-id="bdca0-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdca0-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-endbreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/endbreak

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "end break smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="bdca0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdca0-146">Response</span></span>

<span data-ttu-id="bdca0-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdca0-147">The following is an example of the response.</span></span> 

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
  "description": "End Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
