---
title: 'timeCard: startBreak'
description: Inicie a quebra em um cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 95c220d9b6bcead0f0c734959bb99788e8b5e2fd
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787832"
---
# <a name="timecard-startbreak"></a><span data-ttu-id="4583c-103">timeCard: startBreak</span><span class="sxs-lookup"><span data-stu-id="4583c-103">timeCard: startBreak</span></span>

<span data-ttu-id="4583c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4583c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4583c-105">Inicie uma pausa em um [cartão de ponto específico.](../resources/timeCard.md)</span><span class="sxs-lookup"><span data-stu-id="4583c-105">Start a break in a specific [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4583c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4583c-106">Permissions</span></span>

<span data-ttu-id="4583c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4583c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4583c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4583c-109">Permission type</span></span>      | <span data-ttu-id="4583c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4583c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4583c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4583c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4583c-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4583c-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="4583c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4583c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4583c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4583c-114">Not supported.</span></span>    |
|<span data-ttu-id="4583c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4583c-115">Application</span></span> | <span data-ttu-id="4583c-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="4583c-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="4583c-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="4583c-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="4583c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4583c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/{timeCardID}/startBreak
```

## <a name="request-headers"></a><span data-ttu-id="4583c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4583c-119">Request headers</span></span>

| <span data-ttu-id="4583c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4583c-120">Header</span></span>       | <span data-ttu-id="4583c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4583c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4583c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4583c-122">Authorization</span></span>  | <span data-ttu-id="4583c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4583c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4583c-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4583c-125">Content-type</span></span> | <span data-ttu-id="4583c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4583c-p103">application/json. Required.</span></span>|
| <span data-ttu-id="4583c-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="4583c-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="4583c-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="4583c-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="4583c-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4583c-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4583c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4583c-131">Request body</span></span>

<span data-ttu-id="4583c-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4583c-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4583c-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4583c-133">Parameter</span></span>    | <span data-ttu-id="4583c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="4583c-134">Type</span></span>        | <span data-ttu-id="4583c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="4583c-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4583c-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="4583c-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="4583c-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="4583c-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="4583c-138">notes</span><span class="sxs-lookup"><span data-stu-id="4583c-138">notes</span></span>| [<span data-ttu-id="4583c-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="4583c-139">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="4583c-140">Observações durante o início da pausa.</span><span class="sxs-lookup"><span data-stu-id="4583c-140">Notes during start of break.</span></span>|

## <a name="response"></a><span data-ttu-id="4583c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4583c-141">Response</span></span>

<span data-ttu-id="4583c-142">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4583c-142">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4583c-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4583c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4583c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4583c-144">Request</span></span>
<span data-ttu-id="4583c-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4583c-145">The following is an example of the request.</span></span> 

<!-- {
  "blockType": "request",
  "name": "timecard-startBreak"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/startbreak
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "start break smaple notes"
    }
}
```

### <a name="response"></a><span data-ttu-id="4583c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4583c-146">Response</span></span>

<span data-ttu-id="4583c-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4583c-147">The following is an example of the response.</span></span> 

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
  "description": "Start Break",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
