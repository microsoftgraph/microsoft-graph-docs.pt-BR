---
title: 'Call: rejeitar'
description: Rejeite as chamadas recebidas.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e3befe394aa9451cbb51bd39ba41fb158b67b464
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838828"
---
# <a name="call-reject"></a><span data-ttu-id="27d20-103">Call: rejeitar</span><span class="sxs-lookup"><span data-stu-id="27d20-103">call: reject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d20-104">Permite que o bot rejeite uma [chamada](../resources/call.md)de entrada.</span><span class="sxs-lookup"><span data-stu-id="27d20-104">Enables the bot to reject an incoming [call](../resources/call.md).</span></span> <span data-ttu-id="27d20-105">A solicitação de chamada de entrada pode ser um convite para uma reunião ou uma chamada ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="27d20-105">The incoming call request can be an invite to a meeting or a peer to peer call.</span></span> <span data-ttu-id="27d20-106">A solicitação de chamada de entrada expira após 15 segundos.</span><span class="sxs-lookup"><span data-stu-id="27d20-106">The incoming call request times out after 15 seconds.</span></span> <span data-ttu-id="27d20-107">Se nenhuma resposta for enviada durante esse tempo, a chamada será rejeitada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="27d20-107">If no response is sent during this time, the call is automatically rejected.</span></span>

<span data-ttu-id="27d20-108">Depois que o bot é registrado com uma URL de retorno de chamada válida no portal do Azure, a chamada de entrada é `changeType` entregue como `created`um [commsNotification](../resources/commsnotification.md) com a definição para.</span><span class="sxs-lookup"><span data-stu-id="27d20-108">Once the bot is registered with a valid callback URL in the Azure portal, the incoming call is delivered as a [commsNotification](../resources/commsnotification.md) with `changeType` set to `created`.</span></span> <span data-ttu-id="27d20-109">O bot é esperado `Answer` ou `Reject` a chamada antes que ele expire.</span><span class="sxs-lookup"><span data-stu-id="27d20-109">The bot is expected to `Answer` or `Reject` the call before it times out.</span></span>

> <span data-ttu-id="27d20-110">**Observação:** Essa API é usada apenas para rejeitar chamadas de entrada.</span><span class="sxs-lookup"><span data-stu-id="27d20-110">**Note:** This API is only used to reject incoming calls.</span></span> <span data-ttu-id="27d20-111">Para encerrar as chamadas existentes, a [chamada de exclusão](../api/call-delete.md) deve ser usada em vez disso.</span><span class="sxs-lookup"><span data-stu-id="27d20-111">To terminate existing calls, [Delete Call](../api/call-delete.md) should be used instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d20-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="27d20-112">Permissions</span></span>
<span data-ttu-id="27d20-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27d20-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27d20-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27d20-115">Permission type</span></span> | <span data-ttu-id="27d20-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27d20-116">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="27d20-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27d20-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d20-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="27d20-118">Not Supported</span></span>                       |
| <span data-ttu-id="27d20-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27d20-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d20-120">Não suportado</span><span class="sxs-lookup"><span data-stu-id="27d20-120">Not Supported</span></span>                       |
| <span data-ttu-id="27d20-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27d20-121">Application</span></span>     | <span data-ttu-id="27d20-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27d20-122">None</span></span>                                                       |

## <a name="http-request"></a><span data-ttu-id="27d20-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27d20-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/reject
```

## <a name="request-headers"></a><span data-ttu-id="27d20-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27d20-124">Request headers</span></span>
| <span data-ttu-id="27d20-125">Nome</span><span class="sxs-lookup"><span data-stu-id="27d20-125">Name</span></span>          | <span data-ttu-id="27d20-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="27d20-126">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="27d20-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="27d20-127">Authorization</span></span> | <span data-ttu-id="27d20-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27d20-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27d20-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27d20-130">Request body</span></span>
<span data-ttu-id="27d20-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d20-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27d20-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="27d20-132">Parameter</span></span>      | <span data-ttu-id="27d20-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="27d20-133">Type</span></span>    |<span data-ttu-id="27d20-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="27d20-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27d20-135">motivos</span><span class="sxs-lookup"><span data-stu-id="27d20-135">reason</span></span>|<span data-ttu-id="27d20-136">String</span><span class="sxs-lookup"><span data-stu-id="27d20-136">String</span></span>|<span data-ttu-id="27d20-137">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="27d20-137">The rejection reason.</span></span> <span data-ttu-id="27d20-138">Os valores possíveis `None`são `Busy` e`Forbidden`</span><span class="sxs-lookup"><span data-stu-id="27d20-138">Possible values are `None`, `Busy` and `Forbidden`</span></span> |
|<span data-ttu-id="27d20-139">callbackUri</span><span class="sxs-lookup"><span data-stu-id="27d20-139">callbackUri</span></span>|<span data-ttu-id="27d20-140">String</span><span class="sxs-lookup"><span data-stu-id="27d20-140">String</span></span>|<span data-ttu-id="27d20-141">Permite que os bots forneçam um URI de retorno de chamada específico, onde o resultado da ação de rejeição será lançado.</span><span class="sxs-lookup"><span data-stu-id="27d20-141">Allows bots to provide a specific callback URI where the result of the Reject action will be posted.</span></span> <span data-ttu-id="27d20-142">Isso permite enviar o resultado para a mesma instância de bot específica que disparou a ação rejeitar.</span><span class="sxs-lookup"><span data-stu-id="27d20-142">This allows sending the result to the same specific bot instance that triggered the Reject action.</span></span> <span data-ttu-id="27d20-143">Se nenhum for fornecido, o URI de retorno de chamada global do bot será usado.</span><span class="sxs-lookup"><span data-stu-id="27d20-143">If none is provided, the bot's global callback URI will be used.</span></span>|

## <a name="response"></a><span data-ttu-id="27d20-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d20-144">Response</span></span>
<span data-ttu-id="27d20-p108">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d20-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d20-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27d20-147">Examples</span></span>
<span data-ttu-id="27d20-148">Os exemplos a seguir mostram como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="27d20-148">The following examples shows how to call this API.</span></span>

#### <a name="request"></a><span data-ttu-id="27d20-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d20-149">Request</span></span>
<span data-ttu-id="27d20-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d20-150">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27d20-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d20-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "busy"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27d20-152">C#</span><span class="sxs-lookup"><span data-stu-id="27d20-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27d20-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d20-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27d20-154">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27d20-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)] 

--- 


##### <a name="response"></a><span data-ttu-id="27d20-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d20-155">Response</span></span>
<span data-ttu-id="27d20-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d20-156">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

### <a name="reject-an-incoming-call-with-none-reason"></a><span data-ttu-id="27d20-157">Rejeitar uma chamada de entrada com o motivo ' nenhum '</span><span class="sxs-lookup"><span data-stu-id="27d20-157">Reject an incoming call with 'None' reason</span></span>

##### <a name="notification---incoming"></a><span data-ttu-id="27d20-158">Notificação-entrada</span><span class="sxs-lookup"><span data-stu-id="27d20-158">Notification - incoming</span></span>

```http
POST https://bot.contoso.com/api/call
Authorization: Bearer <TOKEN>
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
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
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

##### <a name="request"></a><span data-ttu-id="27d20-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d20-159">Request</span></span>
<span data-ttu-id="27d20-160">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d20-160">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27d20-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d20-161">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "ignored",
  "name": "call-reject"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject
Content-Type: application/json
Content-Length: 24

{
  "reason": "none"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27d20-162">C#</span><span class="sxs-lookup"><span data-stu-id="27d20-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-reject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27d20-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d20-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-reject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27d20-164">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27d20-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-reject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="27d20-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d20-165">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---deleted"></a><span data-ttu-id="27d20-166">Notificação-excluído</span><span class="sxs-lookup"><span data-stu-id="27d20-166">Notification - deleted</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resource": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57dab8b1-894c-409a-b240-bd8beae78896"
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
