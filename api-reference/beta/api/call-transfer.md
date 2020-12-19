---
title: 'Call: transferência'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7c23ea17f1bc68b88490d8a54a68e50fe0604a78
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719773"
---
# <a name="call-transfer"></a><span data-ttu-id="6330c-103">Call: transferência</span><span class="sxs-lookup"><span data-stu-id="6330c-103">call: transfer</span></span>

<span data-ttu-id="6330c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6330c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6330c-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="6330c-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="6330c-106">**Observação:** Só haverá suporte se o destino transfere e Transfer for usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="6330c-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="6330c-107">A transferência para o número PSTN é suportada apenas para a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="6330c-108">Para saber mais sobre o transferer, o transfere e o destino de transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="6330c-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="6330c-109">Uma transferência consultiva significa que o transferidar pode informar a pessoa para a qual deseja transferir a chamada (o transfere), antes da transferência ser feita.</span><span class="sxs-lookup"><span data-stu-id="6330c-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="6330c-110">Em vez de transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="6330c-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="6330c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6330c-111">Permissions</span></span>
<span data-ttu-id="6330c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6330c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6330c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6330c-114">Permission type</span></span> | <span data-ttu-id="6330c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6330c-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="6330c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6330c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6330c-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6330c-117">Not Supported</span></span>                |
| <span data-ttu-id="6330c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6330c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6330c-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="6330c-119">Not Supported</span></span>                |
| <span data-ttu-id="6330c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6330c-120">Application</span></span>     | <span data-ttu-id="6330c-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="6330c-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="6330c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6330c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="6330c-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="6330c-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="6330c-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="6330c-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6330c-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-125">Request headers</span></span>
| <span data-ttu-id="6330c-126">Nome</span><span class="sxs-lookup"><span data-stu-id="6330c-126">Name</span></span>          | <span data-ttu-id="6330c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6330c-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6330c-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="6330c-128">Authorization</span></span> | <span data-ttu-id="6330c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6330c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6330c-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="6330c-131">Content-type</span></span>  | <span data-ttu-id="6330c-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6330c-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6330c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-134">Request body</span></span>
<span data-ttu-id="6330c-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6330c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6330c-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6330c-136">Parameter</span></span>      | <span data-ttu-id="6330c-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="6330c-137">Type</span></span>    |<span data-ttu-id="6330c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="6330c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6330c-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="6330c-139">transferTarget</span></span>|[<span data-ttu-id="6330c-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6330c-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="6330c-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="6330c-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="6330c-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="6330c-142">clientContext</span></span>|<span data-ttu-id="6330c-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6330c-143">String</span></span>|<span data-ttu-id="6330c-144">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="6330c-144">Unique Client Context string.</span></span> <span data-ttu-id="6330c-145">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="6330c-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="6330c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330c-146">Response</span></span>
<span data-ttu-id="6330c-147">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6330c-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6330c-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6330c-148">Examples</span></span>
<span data-ttu-id="6330c-149">Estes exemplos mostram o fluxo de uma chamada de entrada todo o caminho para os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="6330c-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="6330c-150">Exemplo 1: transferência de chamadas</span><span class="sxs-lookup"><span data-stu-id="6330c-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="6330c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-151">Request</span></span>
<span data-ttu-id="6330c-152">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6330c-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6330c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6330c-153">HTTP</span></span>](#tab/http)
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
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```
# <a name="c"></a>[<span data-ttu-id="6330c-154">C#</span><span class="sxs-lookup"><span data-stu-id="6330c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6330c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6330c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6330c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6330c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6330c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330c-157">Response</span></span>

> <span data-ttu-id="6330c-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6330c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6330c-160">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="6330c-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6330c-161">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="6330c-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="6330c-162">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6330c-163">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="6330c-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6330c-164">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="6330c-164">Notification - transfer failed</span></span>

> <span data-ttu-id="6330c-165">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="6330c-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        }
      }
    }
  ]
}
```

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="6330c-166">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="6330c-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="6330c-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-167">Request</span></span>
<span data-ttu-id="6330c-168">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6330c-168">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="6330c-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330c-169">Response</span></span>

> <span data-ttu-id="6330c-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6330c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6330c-172">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="6330c-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6330c-173">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="6330c-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="6330c-174">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6330c-175">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="6330c-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6330c-176">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="6330c-176">Notification - transfer failed</span></span>

> <span data-ttu-id="6330c-177">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="6330c-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="6330c-178">Exemplo 3: transferência de chamada para o número PSTN</span><span class="sxs-lookup"><span data-stu-id="6330c-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="6330c-179">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="6330c-179">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="6330c-180">Etapa 1: criar instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6330c-180">Step 1: Create application instance</span></span>
<span data-ttu-id="6330c-181">Usando credenciais de administrador de locatário, chame os seguintes cmdlets no PowerShell remoto do locatário para criar a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-181">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="6330c-182">Para obter mais informações, consulte [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6330c-182">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="6330c-183">Etapa 2: atribuir licenças do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6330c-183">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="6330c-184">Use as credenciais de administrador de locatário para entrar https://admin.microsoft.com/ e acessar a guia **usuários-> ativos** .</span><span class="sxs-lookup"><span data-stu-id="6330c-184">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="6330c-185">Selecione a instância do aplicativo, atribua o **plano de chamadas domésticas e internacionais da microsoft 365** e **o Microsoft 365 Phone System-licenças de usuário virtual** e clique em **salvar alterações**.</span><span class="sxs-lookup"><span data-stu-id="6330c-185">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="6330c-186">Se as licenças necessárias não estiverem disponíveis no locatário, você poderá obtê-las na guia **serviços de compra de > de cobrança** .</span><span class="sxs-lookup"><span data-stu-id="6330c-186">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="6330c-187">Etapa 3: adquirir o número PSTN</span><span class="sxs-lookup"><span data-stu-id="6330c-187">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="6330c-188">Use as credenciais de administrador de locatário para entrar no https://admin.teams.microsoft.com/ e clique na guia **portal herdado** no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="6330c-188">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="6330c-189">Na nova página, vá para a guia **números de telefone de > de voz** .</span><span class="sxs-lookup"><span data-stu-id="6330c-189">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="6330c-190">Clique no **+** botão, selecione **novos números de serviço** e vá para a página **Adicionar novos números de serviço** .</span><span class="sxs-lookup"><span data-stu-id="6330c-190">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="6330c-191">Selecione **país/região**, **estado/região**, **cidade**, **quantidade** de entrada e clique em **Adicionar** para pesquisar.</span><span class="sxs-lookup"><span data-stu-id="6330c-191">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="6330c-192">Clique em **adquirir números**.</span><span class="sxs-lookup"><span data-stu-id="6330c-192">Click **acquire numbers**.</span></span> <span data-ttu-id="6330c-193">O número adquirido recentemente será exibido na guia **números de telefone** .</span><span class="sxs-lookup"><span data-stu-id="6330c-193">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="6330c-194">Etapa 4: atribuir o número PSTN à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6330c-194">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="6330c-195">Com as credenciais de administrador de locatário, chame os seguintes cmdlets no PowerShell remoto do locatário para atribuir o número PSTN à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-195">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="6330c-196">Para obter mais informações, consulte [set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6330c-196">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
> <span data-ttu-id="6330c-197">**Observação:** Se um locatário tem números PSTN australianos atribuídos a qualquer instância de aplicativo, essa chamada pode falhar.</span><span class="sxs-lookup"><span data-stu-id="6330c-197">**Note:** If a tenant has Australian PSTN numbers assigned to any application instances, this call might fail.</span></span> <span data-ttu-id="6330c-198">Se um locatário é recém-criado, pode levar alguns dias para que esse recurso esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="6330c-198">If a tenant is newly created, it might take several days for this feature to be available.</span></span>

#### <a name="request"></a><span data-ttu-id="6330c-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-199">Request</span></span>
<span data-ttu-id="6330c-200">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6330c-200">The following example shows the request.</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="6330c-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330c-201">Response</span></span>

> <span data-ttu-id="6330c-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6330c-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6330c-204">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="6330c-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6330c-205">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="6330c-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="6330c-206">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6330c-207">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="6330c-207">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="6330c-208">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="6330c-208">Notification - transfer failed</span></span>

> <span data-ttu-id="6330c-209">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="6330c-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        }
      }
    }
  ]
}
```

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="6330c-210">Exemplo 4: transferência consultiva para o número PSTN</span><span class="sxs-lookup"><span data-stu-id="6330c-210">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="6330c-211">Essa chamada requer uma instância de aplicativo com o número PSTN atribuído, conforme descrito no exemplo 3.</span><span class="sxs-lookup"><span data-stu-id="6330c-211">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

> <span data-ttu-id="6330c-212">**Observação:** Essa chamada pode falhar se um locatário tem números PSTN australianos atribuídos a qualquer instância de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-212">**Note:** This call may fail if a tenant has Australian PSTN numbers assigned to any application instances.</span></span> <span data-ttu-id="6330c-213">Se um locatário é recém-criado, pode levar alguns dias para que esse recurso esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="6330c-213">If a tenant is newly created, it might take several days for this feature to be available.</span></span>


#### <a name="request"></a><span data-ttu-id="6330c-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6330c-214">Request</span></span>
<span data-ttu-id="6330c-215">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6330c-215">The following example shows the request.</span></span>

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
        "phone": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "+12345678901"
        }
    },
    "languageId": "en-us",
    "region": "amer",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  },
  "clientContext": "9e90d1c1-f61e-43e7-9f75-d420159aae08"
}
```

#### <a name="response"></a><span data-ttu-id="6330c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="6330c-216">Response</span></span>

> <span data-ttu-id="6330c-p117">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6330c-p117">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="6330c-219">Notificação-Transferindo</span><span class="sxs-lookup"><span data-stu-id="6330c-219">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="6330c-220">Notificação-transferência aceita</span><span class="sxs-lookup"><span data-stu-id="6330c-220">Notification - transfer accepted</span></span>

> <span data-ttu-id="6330c-221">**Observação:** A transferência aceita pode ocorrer após ou antes do áudio de estado de mídia inativo.</span><span class="sxs-lookup"><span data-stu-id="6330c-221">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="6330c-222">Notificação-transferência concluída</span><span class="sxs-lookup"><span data-stu-id="6330c-222">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="6330c-223">Notificação-falha na transferência</span><span class="sxs-lookup"><span data-stu-id="6330c-223">Notification - transfer failed</span></span>

> <span data-ttu-id="6330c-224">**Observação:** Quando uma transferência de chamada falha, o estado de chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="6330c-224">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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
        }
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


