---
title: 'Call: playPrompt'
description: Reproduza um prompt na chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ad0001c1961f1c6e9126a39609d368104e133aec
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536068"
---
# <a name="call-playprompt"></a><span data-ttu-id="5f08e-103">Call: playPrompt</span><span class="sxs-lookup"><span data-stu-id="5f08e-103">call: playPrompt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f08e-104">Reproduza um prompt na chamada.</span><span class="sxs-lookup"><span data-stu-id="5f08e-104">Play a prompt in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f08e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f08e-105">Permissions</span></span>
<span data-ttu-id="5f08e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f08e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f08e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f08e-108">Permission type</span></span>                        | <span data-ttu-id="5f08e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f08e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f08e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f08e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f08e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f08e-111">Not Supported.</span></span>                               |
| <span data-ttu-id="5f08e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f08e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f08e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f08e-113">Not Supported.</span></span>                               |
| <span data-ttu-id="5f08e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f08e-114">Application</span></span>                            | <span data-ttu-id="5f08e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5f08e-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="5f08e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f08e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/playPrompt
POST /applications/{id}/calls/{id}/playPrompt
```

## <a name="request-headers"></a><span data-ttu-id="5f08e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f08e-117">Request headers</span></span>
| <span data-ttu-id="5f08e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5f08e-118">Name</span></span>          | <span data-ttu-id="5f08e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f08e-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5f08e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f08e-120">Authorization</span></span> | <span data-ttu-id="5f08e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f08e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f08e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f08e-123">Request body</span></span>
<span data-ttu-id="5f08e-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f08e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f08e-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f08e-125">Parameter</span></span>      | <span data-ttu-id="5f08e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f08e-126">Type</span></span>    |<span data-ttu-id="5f08e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f08e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f08e-128">prompts</span><span class="sxs-lookup"><span data-stu-id="5f08e-128">prompts</span></span>|<span data-ttu-id="5f08e-129">coleção [prompt](../resources/prompt.md)</span><span class="sxs-lookup"><span data-stu-id="5f08e-129">[prompt](../resources/prompt.md) collection</span></span>||
|<span data-ttu-id="5f08e-130">clientContext</span><span class="sxs-lookup"><span data-stu-id="5f08e-130">clientContext</span></span>|<span data-ttu-id="5f08e-131">String</span><span class="sxs-lookup"><span data-stu-id="5f08e-131">String</span></span>|<span data-ttu-id="5f08e-132">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="5f08e-132">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="5f08e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f08e-133">Response</span></span>
<span data-ttu-id="5f08e-134">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [playPromptOperation](../resources/playpromptoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f08e-134">If successful, this method returns `200 OK` response code and [playPromptOperation](../resources/playpromptoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f08e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f08e-135">Example</span></span>
<span data-ttu-id="5f08e-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5f08e-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5f08e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f08e-137">Request</span></span>
<span data-ttu-id="5f08e-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f08e-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-playPrompt"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/playPrompt
Content-Type: application/json
Content-Length: 166

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="5f08e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f08e-139">Response</span></span>

> <span data-ttu-id="5f08e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f08e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.playPromptOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5f08e-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5f08e-142">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f08e-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="5f08e-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-playPrompt-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="notification---operation-completed"></a><span data-ttu-id="5f08e-144">Notificação-operação concluída</span><span class="sxs-lookup"><span data-stu-id="5f08e-144">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.playPromptOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: playPrompt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-playprompt.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
