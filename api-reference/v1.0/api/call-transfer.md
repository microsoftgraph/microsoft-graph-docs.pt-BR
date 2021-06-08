---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 2214d4276fc16c198ced411fe125e13389be3480
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52784910"
---
# <a name="call-transfer"></a><span data-ttu-id="56dff-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="56dff-103">call: transfer</span></span>

<span data-ttu-id="56dff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56dff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56dff-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="56dff-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="56dff-106">**Observação:** Isso só será suportado se o destino de transferência e transferência Microsoft Teams usuários que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="56dff-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="56dff-107">Transfer to PSTN number is supported only for application instance.</span><span class="sxs-lookup"><span data-stu-id="56dff-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="56dff-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="56dff-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="56dff-109">Uma transferência consultiva significa que o transferidor pode informar a pessoa para a quem deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="56dff-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="56dff-110">Isso se opõe a transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="56dff-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="56dff-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="56dff-111">Permissions</span></span>
<span data-ttu-id="56dff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56dff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56dff-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56dff-114">Permission type</span></span> | <span data-ttu-id="56dff-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56dff-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="56dff-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56dff-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="56dff-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="56dff-117">Not Supported</span></span>                |
| <span data-ttu-id="56dff-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56dff-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56dff-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="56dff-119">Not Supported</span></span>                |
| <span data-ttu-id="56dff-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56dff-120">Application</span></span>     | <span data-ttu-id="56dff-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="56dff-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="56dff-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56dff-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="56dff-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-123">Request headers</span></span>
| <span data-ttu-id="56dff-124">Nome</span><span class="sxs-lookup"><span data-stu-id="56dff-124">Name</span></span>          | <span data-ttu-id="56dff-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="56dff-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="56dff-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="56dff-126">Authorization</span></span> | <span data-ttu-id="56dff-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56dff-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56dff-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="56dff-129">Content-type</span></span>  | <span data-ttu-id="56dff-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56dff-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="56dff-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-132">Request body</span></span>
<span data-ttu-id="56dff-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56dff-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56dff-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="56dff-134">Parameter</span></span>      | <span data-ttu-id="56dff-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="56dff-135">Type</span></span>    |<span data-ttu-id="56dff-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="56dff-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56dff-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="56dff-137">transferTarget</span></span>|[<span data-ttu-id="56dff-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="56dff-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="56dff-139">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="56dff-139">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="56dff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="56dff-140">Response</span></span>
<span data-ttu-id="56dff-141">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="56dff-141">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="56dff-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56dff-142">Examples</span></span>
<span data-ttu-id="56dff-143">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="56dff-143">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="56dff-144">Exemplo 1: transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="56dff-144">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="56dff-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-145">Request</span></span>
<span data-ttu-id="56dff-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="56dff-146">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56dff-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="56dff-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-1"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="56dff-148">C#</span><span class="sxs-lookup"><span data-stu-id="56dff-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56dff-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56dff-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56dff-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56dff-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56dff-151">Java</span><span class="sxs-lookup"><span data-stu-id="56dff-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56dff-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="56dff-152">Response</span></span>

> <span data-ttu-id="56dff-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56dff-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="56dff-154">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-154">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="56dff-155">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="56dff-155">Notification - transfer accepted</span></span>

> <span data-ttu-id="56dff-156">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="56dff-156">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="56dff-157">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="56dff-157">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="56dff-158">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-158">Notification - transfer failed</span></span>

> <span data-ttu-id="56dff-159">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="56dff-159">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="56dff-160">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="56dff-160">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="56dff-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-161">Request</span></span>
<span data-ttu-id="56dff-162">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="56dff-162">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56dff-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="56dff-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-2"
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="56dff-164">C#</span><span class="sxs-lookup"><span data-stu-id="56dff-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56dff-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56dff-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56dff-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56dff-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56dff-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="56dff-167">Response</span></span>

> <span data-ttu-id="56dff-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56dff-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="56dff-169">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-169">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="56dff-170">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="56dff-170">Notification - transfer accepted</span></span>

> <span data-ttu-id="56dff-171">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="56dff-171">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="56dff-172">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="56dff-172">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="56dff-173">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-173">Notification - transfer failed</span></span>

> <span data-ttu-id="56dff-174">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="56dff-174">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="56dff-175">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="56dff-175">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="56dff-176">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="56dff-176">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="56dff-177">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="56dff-177">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="56dff-178">**Observação:** Telefone ID é o número de telefone no formato E.164.</span><span class="sxs-lookup"><span data-stu-id="56dff-178">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="56dff-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-179">Request</span></span>
<span data-ttu-id="56dff-180">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="56dff-180">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56dff-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="56dff-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-3"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/transfer
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
# <a name="javascript"></a>[<span data-ttu-id="56dff-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56dff-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56dff-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="56dff-183">Response</span></span>

> <span data-ttu-id="56dff-184">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56dff-184">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="56dff-185">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-185">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="56dff-186">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="56dff-186">Notification - transfer accepted</span></span>

> <span data-ttu-id="56dff-187">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="56dff-187">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="56dff-188">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="56dff-188">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="56dff-189">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-189">Notification - transfer failed</span></span>

> <span data-ttu-id="56dff-190">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="56dff-190">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="56dff-191">Exemplo 4: transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="56dff-191">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="56dff-192">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="56dff-192">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="56dff-193">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="56dff-193">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="56dff-194">**Observação:** Telefone ID é o número de telefone no formato E.164.</span><span class="sxs-lookup"><span data-stu-id="56dff-194">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="56dff-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56dff-195">Request</span></span>
<span data-ttu-id="56dff-196">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="56dff-196">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56dff-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="56dff-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-transfer-4"
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
# <a name="javascript"></a>[<span data-ttu-id="56dff-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56dff-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56dff-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="56dff-199">Response</span></span>

> <span data-ttu-id="56dff-200">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="56dff-200">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="56dff-201">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="56dff-202">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="56dff-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="56dff-203">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="56dff-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="56dff-204">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="56dff-204">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="56dff-205">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="56dff-205">Notification - transfer failed</span></span>

> <span data-ttu-id="56dff-206">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="56dff-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

