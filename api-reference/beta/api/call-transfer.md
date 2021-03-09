---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cfd4e0721e43389a03e945db21fb8230a1eb9276
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574878"
---
# <a name="call-transfer"></a><span data-ttu-id="29bfe-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="29bfe-103">call: transfer</span></span>

<span data-ttu-id="29bfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29bfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29bfe-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="29bfe-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="29bfe-106">**Observação:** Isso só será suportado se o destino de transferência e transferência for usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="29bfe-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="29bfe-107">Transfer to PSTN number is supported only for application instance.</span><span class="sxs-lookup"><span data-stu-id="29bfe-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="29bfe-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="29bfe-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="29bfe-109">Uma transferência consultiva significa que o transferidor pode informar a pessoa para a quem deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="29bfe-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="29bfe-110">Isso se opõe a transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="29bfe-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="29bfe-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="29bfe-111">Permissions</span></span>
<span data-ttu-id="29bfe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29bfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29bfe-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29bfe-114">Permission type</span></span> | <span data-ttu-id="29bfe-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29bfe-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="29bfe-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29bfe-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="29bfe-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="29bfe-117">Not Supported</span></span>                |
| <span data-ttu-id="29bfe-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29bfe-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29bfe-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="29bfe-119">Not Supported</span></span>                |
| <span data-ttu-id="29bfe-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29bfe-120">Application</span></span>     | <span data-ttu-id="29bfe-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="29bfe-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="29bfe-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29bfe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="29bfe-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="29bfe-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="29bfe-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="29bfe-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29bfe-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-125">Request headers</span></span>
| <span data-ttu-id="29bfe-126">Nome</span><span class="sxs-lookup"><span data-stu-id="29bfe-126">Name</span></span>          | <span data-ttu-id="29bfe-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="29bfe-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="29bfe-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="29bfe-128">Authorization</span></span> | <span data-ttu-id="29bfe-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29bfe-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="29bfe-131">Content-type</span></span>  | <span data-ttu-id="29bfe-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29bfe-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-134">Request body</span></span>
<span data-ttu-id="29bfe-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bfe-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29bfe-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="29bfe-136">Parameter</span></span>      | <span data-ttu-id="29bfe-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="29bfe-137">Type</span></span>    |<span data-ttu-id="29bfe-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="29bfe-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29bfe-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="29bfe-139">transferTarget</span></span>|[<span data-ttu-id="29bfe-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="29bfe-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="29bfe-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="29bfe-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="29bfe-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="29bfe-142">clientContext</span></span>|<span data-ttu-id="29bfe-143">String</span><span class="sxs-lookup"><span data-stu-id="29bfe-143">String</span></span>|<span data-ttu-id="29bfe-144">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="29bfe-144">Unique Client Context string.</span></span> <span data-ttu-id="29bfe-145">O limite máximo é 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="29bfe-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="29bfe-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bfe-146">Response</span></span>
<span data-ttu-id="29bfe-147">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="29bfe-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="29bfe-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29bfe-148">Examples</span></span>
<span data-ttu-id="29bfe-149">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="29bfe-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="29bfe-150">Exemplo 1: transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="29bfe-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="29bfe-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-151">Request</span></span>
<span data-ttu-id="29bfe-152">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bfe-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="29bfe-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="29bfe-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29bfe-154">C#</span><span class="sxs-lookup"><span data-stu-id="29bfe-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29bfe-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29bfe-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29bfe-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29bfe-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29bfe-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bfe-157">Response</span></span>

> <span data-ttu-id="29bfe-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="29bfe-160">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="29bfe-161">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="29bfe-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="29bfe-162">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="29bfe-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="29bfe-163">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="29bfe-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="29bfe-164">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-164">Notification - transfer failed</span></span>

> <span data-ttu-id="29bfe-165">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="29bfe-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="29bfe-166">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="29bfe-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="29bfe-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-167">Request</span></span>
<span data-ttu-id="29bfe-168">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bfe-168">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="29bfe-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bfe-169">Response</span></span>

> <span data-ttu-id="29bfe-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="29bfe-172">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="29bfe-173">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="29bfe-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="29bfe-174">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="29bfe-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="29bfe-175">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="29bfe-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="29bfe-176">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-176">Notification - transfer failed</span></span>

> <span data-ttu-id="29bfe-177">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="29bfe-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="29bfe-178">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="29bfe-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="29bfe-179">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="29bfe-179">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="29bfe-180">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="29bfe-180">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="29bfe-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-181">Request</span></span>
<span data-ttu-id="29bfe-182">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bfe-182">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="29bfe-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bfe-183">Response</span></span>

> <span data-ttu-id="29bfe-p111">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="29bfe-186">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-186">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="29bfe-187">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="29bfe-187">Notification - transfer accepted</span></span>

> <span data-ttu-id="29bfe-188">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="29bfe-188">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="29bfe-189">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="29bfe-189">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="29bfe-190">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-190">Notification - transfer failed</span></span>

> <span data-ttu-id="29bfe-191">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="29bfe-191">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="29bfe-192">Exemplo 4: transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="29bfe-192">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="29bfe-193">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="29bfe-193">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="29bfe-194">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="29bfe-194">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="29bfe-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29bfe-195">Request</span></span>
<span data-ttu-id="29bfe-196">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bfe-196">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="29bfe-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bfe-197">Response</span></span>

> <span data-ttu-id="29bfe-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29bfe-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="29bfe-200">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-200">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="29bfe-201">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="29bfe-201">Notification - transfer accepted</span></span>

> <span data-ttu-id="29bfe-202">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="29bfe-202">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="29bfe-203">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="29bfe-203">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="29bfe-204">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="29bfe-204">Notification - transfer failed</span></span>

> <span data-ttu-id="29bfe-205">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="29bfe-205">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


