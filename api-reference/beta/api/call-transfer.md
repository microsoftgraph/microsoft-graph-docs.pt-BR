---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: fe54dbb05313fa659e95d2a65e2a9dc74cd1bc83
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047606"
---
# <a name="call-transfer"></a><span data-ttu-id="86cfd-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="86cfd-103">call: transfer</span></span>

<span data-ttu-id="86cfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86cfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86cfd-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="86cfd-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="86cfd-106">**Observação:** Isso só será suportado se o destino de transferência e transferência Microsoft Teams usuários que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="86cfd-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="86cfd-107">Transfer to PSTN number is supported only for application instance.</span><span class="sxs-lookup"><span data-stu-id="86cfd-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="86cfd-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="86cfd-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="86cfd-109">Uma transferência consultiva significa que o transferidor pode informar a pessoa para a quem deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="86cfd-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="86cfd-110">Isso se opõe a transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="86cfd-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="86cfd-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="86cfd-111">Permissions</span></span>
<span data-ttu-id="86cfd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86cfd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86cfd-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86cfd-114">Permission type</span></span> | <span data-ttu-id="86cfd-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86cfd-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="86cfd-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86cfd-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="86cfd-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86cfd-117">Not Supported</span></span>                |
| <span data-ttu-id="86cfd-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86cfd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86cfd-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="86cfd-119">Not Supported</span></span>                |
| <span data-ttu-id="86cfd-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86cfd-120">Application</span></span>     | <span data-ttu-id="86cfd-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="86cfd-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="86cfd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86cfd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="86cfd-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="86cfd-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="86cfd-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="86cfd-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86cfd-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-125">Request headers</span></span>
| <span data-ttu-id="86cfd-126">Nome</span><span class="sxs-lookup"><span data-stu-id="86cfd-126">Name</span></span>          | <span data-ttu-id="86cfd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="86cfd-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="86cfd-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="86cfd-128">Authorization</span></span> | <span data-ttu-id="86cfd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86cfd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="86cfd-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="86cfd-131">Content-type</span></span>  | <span data-ttu-id="86cfd-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86cfd-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86cfd-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-134">Request body</span></span>
<span data-ttu-id="86cfd-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cfd-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="86cfd-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="86cfd-136">Parameter</span></span>      | <span data-ttu-id="86cfd-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="86cfd-137">Type</span></span>    |<span data-ttu-id="86cfd-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="86cfd-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86cfd-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="86cfd-139">transferTarget</span></span>|[<span data-ttu-id="86cfd-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="86cfd-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="86cfd-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="86cfd-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="86cfd-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cfd-142">Response</span></span>
<span data-ttu-id="86cfd-143">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="86cfd-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86cfd-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="86cfd-144">Examples</span></span>
<span data-ttu-id="86cfd-145">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="86cfd-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="86cfd-146">Exemplo 1: transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="86cfd-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="86cfd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-147">Request</span></span>
<span data-ttu-id="86cfd-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cfd-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86cfd-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="86cfd-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="86cfd-150">C#</span><span class="sxs-lookup"><span data-stu-id="86cfd-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86cfd-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86cfd-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86cfd-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86cfd-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86cfd-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cfd-153">Response</span></span>

> <span data-ttu-id="86cfd-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86cfd-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="86cfd-155">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-155">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="86cfd-156">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="86cfd-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="86cfd-157">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="86cfd-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="86cfd-158">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="86cfd-158">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="86cfd-159">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-159">Notification - transfer failed</span></span>

> <span data-ttu-id="86cfd-160">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="86cfd-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="86cfd-161">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="86cfd-161">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="86cfd-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-162">Request</span></span>
<span data-ttu-id="86cfd-163">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cfd-163">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86cfd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="86cfd-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="86cfd-165">C#</span><span class="sxs-lookup"><span data-stu-id="86cfd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86cfd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86cfd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86cfd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86cfd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86cfd-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cfd-168">Response</span></span>

> <span data-ttu-id="86cfd-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86cfd-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="86cfd-170">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-170">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="86cfd-171">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="86cfd-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="86cfd-172">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="86cfd-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="86cfd-173">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="86cfd-173">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="86cfd-174">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-174">Notification - transfer failed</span></span>

> <span data-ttu-id="86cfd-175">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="86cfd-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="86cfd-176">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="86cfd-176">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="86cfd-177">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="86cfd-177">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="86cfd-178">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="86cfd-178">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="86cfd-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-179">Request</span></span>
<span data-ttu-id="86cfd-180">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cfd-180">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86cfd-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="86cfd-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="86cfd-182">C#</span><span class="sxs-lookup"><span data-stu-id="86cfd-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86cfd-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86cfd-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86cfd-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cfd-184">Response</span></span>

> <span data-ttu-id="86cfd-185">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86cfd-185">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="86cfd-186">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-186">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="86cfd-187">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="86cfd-187">Notification - transfer accepted</span></span>

> <span data-ttu-id="86cfd-188">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="86cfd-188">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="86cfd-189">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="86cfd-189">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="86cfd-190">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-190">Notification - transfer failed</span></span>

> <span data-ttu-id="86cfd-191">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="86cfd-191">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="86cfd-192">Exemplo 4: transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="86cfd-192">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="86cfd-193">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="86cfd-193">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="86cfd-194">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="86cfd-194">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>

#### <a name="request"></a><span data-ttu-id="86cfd-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86cfd-195">Request</span></span>
<span data-ttu-id="86cfd-196">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="86cfd-196">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="86cfd-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="86cfd-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="86cfd-198">C#</span><span class="sxs-lookup"><span data-stu-id="86cfd-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86cfd-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86cfd-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86cfd-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="86cfd-200">Response</span></span>

> <span data-ttu-id="86cfd-201">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="86cfd-201">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="86cfd-202">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-202">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="86cfd-203">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="86cfd-203">Notification - transfer accepted</span></span>

> <span data-ttu-id="86cfd-204">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="86cfd-204">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="86cfd-205">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="86cfd-205">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="86cfd-206">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="86cfd-206">Notification - transfer failed</span></span>

> <span data-ttu-id="86cfd-207">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="86cfd-207">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


