---
title: 'Call: rejeitar'
description: Habilitar um bot para rejeitar uma chamada de entrada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 04ec827cce247e6eef57a025ff81a49ae91353d8
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913699"
---
# <a name="call-reject"></a><span data-ttu-id="7e089-103">Call: rejeitar</span><span class="sxs-lookup"><span data-stu-id="7e089-103">call: reject</span></span>

<span data-ttu-id="7e089-104">Habilitar um bot para rejeitar uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="7e089-104">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="7e089-105">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="7e089-105">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="7e089-106">Se for recebido um convite para uma chamada de grupo, a notificação conterá os parâmetros **chatInfo** e **meetingInfo** .</span><span class="sxs-lookup"><span data-stu-id="7e089-106">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="7e089-107">O bot deve responder ou rejeitar a chamada antes do tempo limite da chamada. O valor de tempo limite atual é de 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="7e089-107">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="7e089-108">Esta API não termina chamadas existentes que já foram respondidas.</span><span class="sxs-lookup"><span data-stu-id="7e089-108">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="7e089-109">Use [delete Call](../api/call-delete.md) para encerrar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="7e089-109">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e089-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e089-110">Permissions</span></span>
<span data-ttu-id="7e089-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e089-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e089-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e089-113">Permission type</span></span> | <span data-ttu-id="7e089-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e089-114">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="7e089-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e089-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e089-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7e089-116">Not Supported</span></span>                       |
| <span data-ttu-id="7e089-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e089-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e089-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7e089-118">Not Supported</span></span>                       |
| <span data-ttu-id="7e089-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e089-119">Application</span></span>     | <span data-ttu-id="7e089-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e089-120">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="7e089-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e089-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="7e089-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e089-122">Request headers</span></span>
| <span data-ttu-id="7e089-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7e089-123">Name</span></span>          | <span data-ttu-id="7e089-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e089-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7e089-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e089-125">Authorization</span></span> | <span data-ttu-id="7e089-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e089-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e089-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="7e089-128">Content-type</span></span>  | <span data-ttu-id="7e089-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e089-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e089-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e089-131">Request body</span></span>
<span data-ttu-id="7e089-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e089-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e089-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7e089-133">Parameter</span></span>      | <span data-ttu-id="7e089-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e089-134">Type</span></span>    |<span data-ttu-id="7e089-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e089-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e089-136">motivo</span><span class="sxs-lookup"><span data-stu-id="7e089-136">reason</span></span>|<span data-ttu-id="7e089-137">String</span><span class="sxs-lookup"><span data-stu-id="7e089-137">String</span></span>|<span data-ttu-id="7e089-138">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="7e089-138">The rejection reason.</span></span> <span data-ttu-id="7e089-139">Os valores possíveis `None`são `Busy` e`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="7e089-139">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="7e089-140">callbackUri</span><span class="sxs-lookup"><span data-stu-id="7e089-140">callbackUri</span></span>|<span data-ttu-id="7e089-141">String</span><span class="sxs-lookup"><span data-stu-id="7e089-141">String</span></span>|<span data-ttu-id="7e089-142">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="7e089-142">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="7e089-143">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="7e089-143">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="7e089-144">Deve ser `https`.</span><span class="sxs-lookup"><span data-stu-id="7e089-144">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="7e089-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e089-145">Response</span></span>
<span data-ttu-id="7e089-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e089-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e089-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e089-148">Examples</span></span>
<span data-ttu-id="7e089-149">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7e089-149">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="7e089-150">Exemplo 1: rejeitar uma chamada de entrada com o motivo "ocupado"</span><span class="sxs-lookup"><span data-stu-id="7e089-150">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="7e089-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e089-151">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e089-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e089-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e089-153">C#</span><span class="sxs-lookup"><span data-stu-id="7e089-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e089-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e089-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e089-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e089-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javatabjava"></a>[<span data-ttu-id="7e089-156">Java</span><span class="sxs-lookup"><span data-stu-id="7e089-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="7e089-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e089-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="7e089-158">Exemplo 2: rejeitar uma chamada de entrada com o motivo ' nenhum '</span><span class="sxs-lookup"><span data-stu-id="7e089-158">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="7e089-159">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="7e089-159">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "name": "call-reject-none",
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
            }
          }
        ],
        "requestedModalities": [ "audio", "video" ]
      }
    }
  ]
}
```

##### <a name="request"></a><span data-ttu-id="7e089-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e089-160">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7e089-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e089-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject-none-reason"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e089-162">C#</span><span class="sxs-lookup"><span data-stu-id="7e089-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e089-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e089-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e089-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e089-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7e089-165">Java</span><span class="sxs-lookup"><span data-stu-id="7e089-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e089-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e089-166">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="7e089-167">Notificação-excluído</span><span class="sxs-lookup"><span data-stu-id="7e089-167">Notification - deleted</span></span>

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
