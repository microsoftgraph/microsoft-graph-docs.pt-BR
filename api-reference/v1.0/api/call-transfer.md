---
title: 'Call: transferência'
description: Transferir uma chamada ponto a ponto ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 940c3a7fb1e2f1320e2598d379bd659cec2c1710
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865709"
---
# <a name="call-transfer"></a><span data-ttu-id="dc08e-103">Call: transferência</span><span class="sxs-lookup"><span data-stu-id="dc08e-103">call: transfer</span></span>

<span data-ttu-id="dc08e-104">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="dc08e-104">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="dc08e-105">**Observação:** Só haverá suporte se o destino transfere e Transfer for usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="dc08e-105">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="dc08e-106">A transferência para o número PSTN não é suportada.</span><span class="sxs-lookup"><span data-stu-id="dc08e-106">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="dc08e-107">Para saber mais sobre o transferer, o transfere e o destino de transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="dc08e-107">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="dc08e-108">Uma transferência consultiva significa que o transferidar pode informar a pessoa para a qual deseja transferir a chamada (o transfere), antes da transferência ser feita.</span><span class="sxs-lookup"><span data-stu-id="dc08e-108">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="dc08e-109">Em vez de transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="dc08e-109">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc08e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc08e-110">Permissions</span></span>
<span data-ttu-id="dc08e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc08e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc08e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc08e-113">Permission type</span></span> | <span data-ttu-id="dc08e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc08e-114">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="dc08e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc08e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc08e-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dc08e-116">Not Supported</span></span>                |
| <span data-ttu-id="dc08e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc08e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc08e-118">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dc08e-118">Not Supported</span></span>                |
| <span data-ttu-id="dc08e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc08e-119">Application</span></span>     | <span data-ttu-id="dc08e-120">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="dc08e-120">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="dc08e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc08e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="dc08e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc08e-122">Request headers</span></span>
| <span data-ttu-id="dc08e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="dc08e-123">Name</span></span>          | <span data-ttu-id="dc08e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc08e-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dc08e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc08e-125">Authorization</span></span> | <span data-ttu-id="dc08e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc08e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc08e-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="dc08e-128">Content-type</span></span>  | <span data-ttu-id="dc08e-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc08e-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc08e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc08e-131">Request body</span></span>
<span data-ttu-id="dc08e-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc08e-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc08e-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dc08e-133">Parameter</span></span>      | <span data-ttu-id="dc08e-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc08e-134">Type</span></span>    |<span data-ttu-id="dc08e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc08e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc08e-136">transferTarget</span><span class="sxs-lookup"><span data-stu-id="dc08e-136">transferTarget</span></span>|[<span data-ttu-id="dc08e-137">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="dc08e-137">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="dc08e-138">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="dc08e-138">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="dc08e-139">clientContext</span><span class="sxs-lookup"><span data-stu-id="dc08e-139">clientContext</span></span>|<span data-ttu-id="dc08e-140">String</span><span class="sxs-lookup"><span data-stu-id="dc08e-140">String</span></span>|<span data-ttu-id="dc08e-141">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="dc08e-141">Unique Client Context string.</span></span> <span data-ttu-id="dc08e-142">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="dc08e-142">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="dc08e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc08e-143">Response</span></span>
<span data-ttu-id="dc08e-144">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="dc08e-144">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dc08e-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dc08e-145">Examples</span></span>
<span data-ttu-id="dc08e-146">Estes exemplos mostram o fluxo de uma chamada de entrada todo o caminho para os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="dc08e-146">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="dc08e-147">Exemplo 1: transferência de chamadas</span><span class="sxs-lookup"><span data-stu-id="dc08e-147">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="dc08e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc08e-148">Request</span></span>
<span data-ttu-id="dc08e-149">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc08e-149">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc08e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc08e-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/transfer
Content-Type: application/json
Content-Length: 430

{
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "replacesCallId-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc08e-151">C#</span><span class="sxs-lookup"><span data-stu-id="dc08e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc08e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc08e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc08e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc08e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc08e-154">Java</span><span class="sxs-lookup"><span data-stu-id="dc08e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc08e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc08e-155">Response</span></span>

> <span data-ttu-id="dc08e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc08e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="dc08e-158">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="dc08e-158">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="dc08e-159">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="dc08e-159">Notification - transfer accepted</span></span>

> <span data-ttu-id="dc08e-160">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="dc08e-160">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="dc08e-161">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="dc08e-161">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="dc08e-162">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="dc08e-162">Notification - transfer failed</span></span>

> <span data-ttu-id="dc08e-163">**Observação:** Quando uma transferência de chamada falha, o estado de chamada `established`será.</span><span class="sxs-lookup"><span data-stu-id="dc08e-163">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="dc08e-164">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="dc08e-164">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="dc08e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc08e-165">Request</span></span>
<span data-ttu-id="dc08e-166">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc08e-166">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "@odata.type": "call-transfer"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/341a0500-d4bf-4224-8b19-1581168d328b/transfer
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
        "displayName": "Heidi Steen"
      }
    },
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

##### <a name="response"></a><span data-ttu-id="dc08e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc08e-167">Response</span></span>

> <span data-ttu-id="dc08e-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc08e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="dc08e-170">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="dc08e-170">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="dc08e-171">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="dc08e-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="dc08e-172">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="dc08e-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="dc08e-173">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="dc08e-173">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="dc08e-174">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="dc08e-174">Notification - transfer failed</span></span>

> <span data-ttu-id="dc08e-175">**Observação:** Quando uma transferência de chamada falha, o estado de chamada `established`será.</span><span class="sxs-lookup"><span data-stu-id="dc08e-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
