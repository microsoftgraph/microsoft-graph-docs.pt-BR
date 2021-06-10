---
title: 'timeCard: clockIn'
description: Entre para iniciar um cartão de ponto.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a21d1fd3af16b342ffcc98c47d854cf49a00ccd
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869797"
---
# <a name="timecard-clockin"></a><span data-ttu-id="ca6a1-103">timeCard: clockIn</span><span class="sxs-lookup"><span data-stu-id="ca6a1-103">timeCard: clockIn</span></span>

<span data-ttu-id="ca6a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca6a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca6a1-105">Clock in to start a [timeCard](../resources/timeCard.md).</span><span class="sxs-lookup"><span data-stu-id="ca6a1-105">Clock in to start a [timeCard](../resources/timeCard.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca6a1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ca6a1-106">Permissions</span></span>

<span data-ttu-id="ca6a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca6a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca6a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca6a1-109">Permission type</span></span>      | <span data-ttu-id="ca6a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca6a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca6a1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca6a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca6a1-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca6a1-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca6a1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca6a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca6a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-114">Not supported.</span></span>    |
|<span data-ttu-id="ca6a1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca6a1-115">Application</span></span> | <span data-ttu-id="ca6a1-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="ca6a1-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="ca6a1-117">\***Importante:** Quando você usa permissões de aplicativo, deve incluir `MS-APP-ACTS-AS` o header na solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca6a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6a1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards/clockIn
```

## <a name="request-headers"></a><span data-ttu-id="ca6a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6a1-119">Request headers</span></span>

| <span data-ttu-id="ca6a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca6a1-120">Header</span></span>       | <span data-ttu-id="ca6a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca6a1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca6a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca6a1-122">Authorization</span></span>  | <span data-ttu-id="ca6a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ca6a1-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="ca6a1-125">Content-type</span></span> | <span data-ttu-id="ca6a1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-p103">application/json. Required.</span></span>|
| <span data-ttu-id="ca6a1-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="ca6a1-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="ca6a1-129">A ID do usuário em nome do qual o aplicativo está agindo.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="ca6a1-130">Obrigatório ao usar o escopo de permissão do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca6a1-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6a1-131">Request body</span></span>

<span data-ttu-id="ca6a1-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca6a1-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ca6a1-133">Parameter</span></span>    | <span data-ttu-id="ca6a1-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca6a1-134">Type</span></span>        | <span data-ttu-id="ca6a1-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca6a1-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca6a1-136">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="ca6a1-136">atApprovedLocation</span></span>| `Edm.boolean ` | <span data-ttu-id="ca6a1-137">Indique se essa ação acontece em um local aprovado.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-137">Indicate if this action happens at an approved location.</span></span>|
|<span data-ttu-id="ca6a1-138">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="ca6a1-138">onBehalfOfUserId</span></span>| <span data-ttu-id="ca6a1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca6a1-139">String</span></span> | <span data-ttu-id="ca6a1-140">Parâmetro opcional usado pelo gerente para entrar no relógio em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-140">Optional parameter used by the manager to clock in on behalf of a user.</span></span>|
|<span data-ttu-id="ca6a1-141">notes</span><span class="sxs-lookup"><span data-stu-id="ca6a1-141">notes</span></span>| [<span data-ttu-id="ca6a1-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="ca6a1-142">itemBody</span></span>](../resources/itembody.md)  |<span data-ttu-id="ca6a1-143">Observações para o relógio em.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-143">Notes for the clock in.</span></span> |

## <a name="response"></a><span data-ttu-id="ca6a1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6a1-144">Response</span></span>

<span data-ttu-id="ca6a1-145">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [timeCard](../resources/timeCard.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-145">If successful, this method returns a `201 Created` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca6a1-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca6a1-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca6a1-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca6a1-147">Request</span></span>
<span data-ttu-id="ca6a1-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-148">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="ca6a1-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca6a1-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-clockin"
}-->

```http
POST https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/clockin
Content-type: application/json

{
    "atAprovedLocation": true,
    "notes": {
        "contentType": "text",
        "content": "clock in notes"
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="ca6a1-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca6a1-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-clockin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca6a1-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca6a1-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-clockin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca6a1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca6a1-152">Response</span></span>

<span data-ttu-id="ca6a1-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-153">The following is an example of the response.</span></span> 

><span data-ttu-id="ca6a1-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca6a1-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T22:58:41.327Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedIn",
    "confirmedBy": "none",
    "clockOutEvent": null,
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "breaks": [],
    "originalEntry": {
        "clockOutEvent": null,
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "breaks": []
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Clock In",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
