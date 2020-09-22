---
title: 'Call: transferência'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 3c4fc0e6b104e1888199f8323b787333b57b75d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987285"
---
# <a name="call-transfer"></a><span data-ttu-id="75b34-103">Call: transferência</span><span class="sxs-lookup"><span data-stu-id="75b34-103">call: transfer</span></span>

<span data-ttu-id="75b34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75b34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b34-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="75b34-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="75b34-106">**Observação:** Só haverá suporte se o destino transfere e Transfer for usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="75b34-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="75b34-107">A transferência para o número PSTN não é suportada.</span><span class="sxs-lookup"><span data-stu-id="75b34-107">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="75b34-108">Para saber mais sobre o transferer, o transfere e o destino de transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="75b34-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="75b34-109">Uma transferência consultiva significa que o transferidar pode informar a pessoa para a qual deseja transferir a chamada (o transfere), antes da transferência ser feita.</span><span class="sxs-lookup"><span data-stu-id="75b34-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="75b34-110">Em vez de transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="75b34-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="75b34-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="75b34-111">Permissions</span></span>
<span data-ttu-id="75b34-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b34-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75b34-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75b34-114">Permission type</span></span> | <span data-ttu-id="75b34-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75b34-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="75b34-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75b34-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="75b34-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="75b34-117">Not Supported</span></span>                |
| <span data-ttu-id="75b34-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75b34-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75b34-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="75b34-119">Not Supported</span></span>                |
| <span data-ttu-id="75b34-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75b34-120">Application</span></span>     | <span data-ttu-id="75b34-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="75b34-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="75b34-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75b34-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="75b34-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="75b34-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="75b34-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="75b34-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75b34-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75b34-125">Request headers</span></span>
| <span data-ttu-id="75b34-126">Nome</span><span class="sxs-lookup"><span data-stu-id="75b34-126">Name</span></span>          | <span data-ttu-id="75b34-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="75b34-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="75b34-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="75b34-128">Authorization</span></span> | <span data-ttu-id="75b34-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75b34-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="75b34-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="75b34-131">Content-type</span></span>  | <span data-ttu-id="75b34-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75b34-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75b34-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75b34-134">Request body</span></span>
<span data-ttu-id="75b34-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75b34-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="75b34-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="75b34-136">Parameter</span></span>      | <span data-ttu-id="75b34-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="75b34-137">Type</span></span>    |<span data-ttu-id="75b34-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="75b34-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75b34-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="75b34-139">transferTarget</span></span>|[<span data-ttu-id="75b34-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="75b34-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="75b34-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="75b34-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="75b34-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="75b34-142">clientContext</span></span>|<span data-ttu-id="75b34-143">String</span><span class="sxs-lookup"><span data-stu-id="75b34-143">String</span></span>|<span data-ttu-id="75b34-144">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="75b34-144">Unique Client Context string.</span></span> <span data-ttu-id="75b34-145">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="75b34-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="75b34-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="75b34-146">Response</span></span>
<span data-ttu-id="75b34-147">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="75b34-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="75b34-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="75b34-148">Examples</span></span>
<span data-ttu-id="75b34-149">Estes exemplos mostram o fluxo de uma chamada de entrada todo o caminho para os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="75b34-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="75b34-150">Exemplo 1: transferência de chamadas</span><span class="sxs-lookup"><span data-stu-id="75b34-150">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="75b34-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75b34-151">Request</span></span>
<span data-ttu-id="75b34-152">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="75b34-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75b34-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="75b34-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value",
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="75b34-154">C#</span><span class="sxs-lookup"><span data-stu-id="75b34-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75b34-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75b34-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75b34-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75b34-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="75b34-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="75b34-157">Response</span></span>

> <span data-ttu-id="75b34-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75b34-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="75b34-160">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="75b34-160">Notification - transferring</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="75b34-161">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="75b34-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="75b34-162">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="75b34-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

##### <a name="notification---transfer-completed"></a><span data-ttu-id="75b34-163">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="75b34-163">Notification - transfer completed</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 0,
          "subcode": 7015,
          "message": "GracefulTransferCompleted"
        }
      }
    }
  ]
}
```

##### <a name="notification---transfer-failed"></a><span data-ttu-id="75b34-164">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="75b34-164">Notification - transfer failed</span></span>

> <span data-ttu-id="75b34-165">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="75b34-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7000,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="75b34-166">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="75b34-166">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="75b34-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75b34-167">Request</span></span>
<span data-ttu-id="75b34-168">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="75b34-168">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
Content-Type: application/json

{
  "transferTarget": {
    "@odata.type": "#microsoft.graph.invitationParticipantInfo",
    "endpointType": "default",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

##### <a name="response"></a><span data-ttu-id="75b34-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="75b34-169">Response</span></span>

> <span data-ttu-id="75b34-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75b34-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="75b34-172">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="75b34-172">Notification - transferring</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferring"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="75b34-173">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="75b34-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="75b34-174">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="75b34-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "transferAccepted"
      }
    }
  ]
}
```

##### <a name="notification---transfer-completed"></a><span data-ttu-id="75b34-175">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="75b34-175">Notification - transfer completed</span></span>

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
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

##### <a name="notification---transfer-failed"></a><span data-ttu-id="75b34-176">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="75b34-176">Notification - transfer failed</span></span>

> <span data-ttu-id="75b34-177">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="75b34-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
      "changeType": "updated",
      "resourceUrl": "/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "established",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": 500,
          "subCode": 7700,
          "message": "<message>"
        },
        "replacesContext": "<replacesContext>"
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
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


