---
title: 'call: reject'
description: Habilitar um bot para rejeitar uma chamada de entrada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1355a826ab3bfaeea3392e20a6e40c71a279ca58
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787489"
---
# <a name="call-reject"></a><span data-ttu-id="711e9-103">call: reject</span><span class="sxs-lookup"><span data-stu-id="711e9-103">call: reject</span></span>

<span data-ttu-id="711e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="711e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="711e9-105">Habilitar um bot para rejeitar uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="711e9-105">Enable a bot to reject an incoming call.</span></span> <span data-ttu-id="711e9-106">A solicitação de chamada de entrada pode ser um convite de um participante em uma chamada de grupo ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="711e9-106">The incoming call request can be an invite from a participant in a group call or a peer-to-peer call.</span></span> <span data-ttu-id="711e9-107">Se um convite para uma chamada de grupo for recebido, a notificação conterá os parâmetros **chatInfo** e **meetingInfo.**</span><span class="sxs-lookup"><span data-stu-id="711e9-107">If an invite to a group call is received, the notification will contain the **chatInfo** and **meetingInfo** parameters.</span></span>

<span data-ttu-id="711e9-108">Espera-se que o bot atenda ou rejeite a chamada antes do tempo de chamada. O valor de tempo decoro atual é 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="711e9-108">The bot is expected to answer or reject the call before the call times out. The current timeout value is 15 seconds.</span></span>

<span data-ttu-id="711e9-109">Essa API não termina chamadas existentes que já foram atendidas.</span><span class="sxs-lookup"><span data-stu-id="711e9-109">This API does not end existing calls that have already been answered.</span></span> <span data-ttu-id="711e9-110">Use [excluir chamada para](../api/call-delete.md) encerrar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="711e9-110">Use [delete call](../api/call-delete.md) to end a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="711e9-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="711e9-111">Permissions</span></span>
<span data-ttu-id="711e9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="711e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="711e9-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="711e9-114">Permission type</span></span> | <span data-ttu-id="711e9-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="711e9-115">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="711e9-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="711e9-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="711e9-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="711e9-117">Not Supported</span></span>                       |
| <span data-ttu-id="711e9-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="711e9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="711e9-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="711e9-119">Not Supported</span></span>                       |
| <span data-ttu-id="711e9-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="711e9-120">Application</span></span>     | <span data-ttu-id="711e9-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="711e9-121">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="711e9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="711e9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="711e9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="711e9-123">Request headers</span></span>
| <span data-ttu-id="711e9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="711e9-124">Name</span></span>          | <span data-ttu-id="711e9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="711e9-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="711e9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="711e9-126">Authorization</span></span> | <span data-ttu-id="711e9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="711e9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="711e9-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="711e9-129">Content-type</span></span>  | <span data-ttu-id="711e9-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="711e9-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="711e9-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="711e9-132">Request body</span></span>
<span data-ttu-id="711e9-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="711e9-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="711e9-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="711e9-134">Parameter</span></span>      | <span data-ttu-id="711e9-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="711e9-135">Type</span></span>    |<span data-ttu-id="711e9-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="711e9-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711e9-137">motivo</span><span class="sxs-lookup"><span data-stu-id="711e9-137">reason</span></span>|<span data-ttu-id="711e9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="711e9-138">String</span></span>|<span data-ttu-id="711e9-139">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="711e9-139">The rejection reason.</span></span> <span data-ttu-id="711e9-140">Os valores possíveis `None` são e `Busy``Forbidden`</span><span class="sxs-lookup"><span data-stu-id="711e9-140">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="711e9-141">callbackUri</span><span class="sxs-lookup"><span data-stu-id="711e9-141">callbackUri</span></span>|<span data-ttu-id="711e9-142">String</span><span class="sxs-lookup"><span data-stu-id="711e9-142">String</span></span>|<span data-ttu-id="711e9-143">Isso permite que os bots forneçam um URI de retorno de chamada específico para que a chamada atual receba notificações posteriores.</span><span class="sxs-lookup"><span data-stu-id="711e9-143">This allows bots to provide a specific callback URI for the current call to receive later notifications.</span></span> <span data-ttu-id="711e9-144">Se essa propriedade não tiver sido definida, o URI de retorno de chamada global do bot será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="711e9-144">If this property has not been set, the bot's global callback URI will be used instead.</span></span> <span data-ttu-id="711e9-145">Isso deve ser `https` .</span><span class="sxs-lookup"><span data-stu-id="711e9-145">This must be `https`.</span></span>|

## <a name="response"></a><span data-ttu-id="711e9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="711e9-146">Response</span></span>
<span data-ttu-id="711e9-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="711e9-p108">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="711e9-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="711e9-149">Examples</span></span>
<span data-ttu-id="711e9-150">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="711e9-150">The following examples show how to call this API.</span></span>

### <a name="example-1-reject-an-incoming-call-with-busy-reason"></a><span data-ttu-id="711e9-151">Exemplo 1: rejeitar uma chamada de entrada com motivo "Ocupado"</span><span class="sxs-lookup"><span data-stu-id="711e9-151">Example 1: Reject an incoming call with 'Busy' reason</span></span>
#### <a name="request"></a><span data-ttu-id="711e9-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="711e9-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="711e9-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="711e9-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="711e9-154">C#</span><span class="sxs-lookup"><span data-stu-id="711e9-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascript"></a>[<span data-ttu-id="711e9-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="711e9-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-c"></a>[<span data-ttu-id="711e9-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="711e9-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="java"></a>[<span data-ttu-id="711e9-157">Java</span><span class="sxs-lookup"><span data-stu-id="711e9-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

--- 


##### <a name="response"></a><span data-ttu-id="711e9-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="711e9-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="711e9-159">Exemplo 2: rejeitar uma chamada de entrada com motivo 'Nenhum'</span><span class="sxs-lookup"><span data-stu-id="711e9-159">Example 2: Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="711e9-160">Notificação - entrada</span><span class="sxs-lookup"><span data-stu-id="711e9-160">Notification - incoming</span></span>

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

##### <a name="request"></a><span data-ttu-id="711e9-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="711e9-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="711e9-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="711e9-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="711e9-163">C#</span><span class="sxs-lookup"><span data-stu-id="711e9-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-none-reason-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="711e9-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="711e9-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-none-reason-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="711e9-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="711e9-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-none-reason-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="711e9-166">Java</span><span class="sxs-lookup"><span data-stu-id="711e9-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-reject-none-reason-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="711e9-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="711e9-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="711e9-168">Notificação - excluída</span><span class="sxs-lookup"><span data-stu-id="711e9-168">Notification - deleted</span></span>

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

