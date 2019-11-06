---
title: 'Call: rejeitar'
description: Habilitar um bot para rejeitar uma chamada de entrada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a083459a162117addba494f74e50842435a74516
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38005903"
---
# <a name="call-reject"></a><span data-ttu-id="47962-103">Call: rejeitar</span><span class="sxs-lookup"><span data-stu-id="47962-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47962-104">Habilitar um bot para rejeitar uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="47962-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="47962-105">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="47962-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="47962-106">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros **chatInfo** e **meetingInfo** .</span><span class="sxs-lookup"><span data-stu-id="47962-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="47962-107">O bot deve responder ou rejeitar a chamada antes do tempo limite da chamada. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="47962-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="47962-108">Esta API não termina chamadas existentes que já foram respondidas.</span><span class="sxs-lookup"><span data-stu-id="47962-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="47962-109">Use [delete Call](../api/call-delete.md) para encerrar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="47962-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

> <span data-ttu-id="47962-110">**Observação:** O bot só pode ser alcançado por meio de VoIP.</span><span class="sxs-lookup"><span data-stu-id="47962-110">**Note:** The bot can only be reached through VoIP.</span></span> <span data-ttu-id="47962-111">A chamada PSTN para Bot ainda não é suportada.</span><span class="sxs-lookup"><span data-stu-id="47962-111">PSTN calling to bot is not yet supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="47962-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="47962-112">Permissions</span></span>
<span data-ttu-id="47962-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47962-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47962-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47962-115">Permission type</span></span> | <span data-ttu-id="47962-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47962-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="47962-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47962-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="47962-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="47962-118">Not Supported</span></span>                       |
| <span data-ttu-id="47962-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47962-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47962-120">Não suportado</span><span class="sxs-lookup"><span data-stu-id="47962-120">Not Supported</span></span>                       |
| <span data-ttu-id="47962-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47962-121">Application</span></span>     | <span data-ttu-id="47962-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47962-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="47962-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47962-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
POST /communications/calls/{id}/reject
```
> <span data-ttu-id="47962-124">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="47962-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="47962-125">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="47962-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47962-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47962-126">Request headers</span></span>
| <span data-ttu-id="47962-127">Nome</span><span class="sxs-lookup"><span data-stu-id="47962-127">Name</span></span>          | <span data-ttu-id="47962-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="47962-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="47962-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="47962-129">Authorization</span></span> | <span data-ttu-id="47962-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47962-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47962-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="47962-132">Content-type</span></span>  | <span data-ttu-id="47962-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47962-p107">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47962-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47962-135">Request body</span></span>
<span data-ttu-id="47962-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47962-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47962-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="47962-137">Parameter</span></span>      | <span data-ttu-id="47962-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="47962-138">Type</span></span>    |<span data-ttu-id="47962-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="47962-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47962-140">motivo</span><span class="sxs-lookup"><span data-stu-id="47962-140">reason</span></span>|<span data-ttu-id="47962-141">String</span><span class="sxs-lookup"><span data-stu-id="47962-141">String</span></span>|<span data-ttu-id="47962-142">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="47962-142">The rejection reason.</span></span> <span data-ttu-id="47962-143">Os valores possíveis `None`são `Busy` e`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="47962-143">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="47962-144">callbackUri</span><span class="sxs-lookup"><span data-stu-id="47962-144">callbackUri</span></span>|<span data-ttu-id="47962-145">String</span><span class="sxs-lookup"><span data-stu-id="47962-145">String</span></span>|<span data-ttu-id="47962-146">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="47962-146">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="47962-147">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="47962-147">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="47962-148">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="47962-148">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="47962-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="47962-149">Response</span></span>
<span data-ttu-id="47962-p110">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47962-p110">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47962-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47962-152">Examples</span></span>
<span data-ttu-id="47962-153">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="47962-153">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="47962-154">Exemplo 1: rejeitar uma chamada de entrada com o motivo "ocupado"</span><span class="sxs-lookup"><span data-stu-id="47962-154">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="47962-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47962-155">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47962-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="47962-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47962-157">C#</span><span class="sxs-lookup"><span data-stu-id="47962-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47962-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47962-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47962-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47962-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="47962-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="47962-160">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="47962-161">Exemplo 2: rejeitar uma chamada de entrada com o motivo ' nenhum '</span><span class="sxs-lookup"><span data-stu-id="47962-161">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="47962-162">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="47962-162">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
        "state": "incoming",
        "direction": "incoming",
        "source": {
          "identity": {
            "user": {
              "displayName": "John",
              "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
            }
          },
          "region": "westus",
          "languageId": "en-US"
        },
        "targets": [
          {
            "identity": {
              "application": {
                "displayName": "Calling Bot",
                "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
              }
            },
            "region": "westus",
            "languageId": "en-US"
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="47962-163">Solicitar</span><span class="sxs-lookup"><span data-stu-id="47962-163">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```

##### <a name="response"></a><span data-ttu-id="47962-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="47962-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="47962-165">Notificação-excluído</span><span class="sxs-lookup"><span data-stu-id="47962-165">Notification - deleted</span></span>

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896"
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
  "description": "call: reject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
