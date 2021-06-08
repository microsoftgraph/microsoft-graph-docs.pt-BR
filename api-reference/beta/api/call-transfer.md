---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6b4a9c00bc40f2bfd0ea9cc40317c426f2c2aa2c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786553"
---
# <a name="call-transfer"></a><span data-ttu-id="2c03d-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="2c03d-103">call: transfer</span></span>

<span data-ttu-id="2c03d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c03d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c03d-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="2c03d-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="2c03d-106">**Observação:** Isso só será suportado se o destino de transferência e transferência Microsoft Teams usuários que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="2c03d-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="2c03d-107">Transfer to PSTN number is supported only for application instance.</span><span class="sxs-lookup"><span data-stu-id="2c03d-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="2c03d-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="2c03d-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="2c03d-109">Uma transferência consultiva significa que o transferidor pode informar a pessoa para a quem deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="2c03d-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="2c03d-110">Isso se opõe a transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="2c03d-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c03d-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c03d-111">Permissions</span></span>
<span data-ttu-id="2c03d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c03d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c03d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c03d-114">Permission type</span></span> | <span data-ttu-id="2c03d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c03d-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="2c03d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c03d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c03d-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2c03d-117">Not Supported</span></span>                |
| <span data-ttu-id="2c03d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c03d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c03d-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2c03d-119">Not Supported</span></span>                |
| <span data-ttu-id="2c03d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c03d-120">Application</span></span>     | <span data-ttu-id="2c03d-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="2c03d-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="2c03d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c03d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="2c03d-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="2c03d-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="2c03d-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="2c03d-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c03d-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-125">Request headers</span></span>
| <span data-ttu-id="2c03d-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2c03d-126">Name</span></span>          | <span data-ttu-id="2c03d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c03d-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2c03d-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c03d-128">Authorization</span></span> | <span data-ttu-id="2c03d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c03d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c03d-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="2c03d-131">Content-type</span></span>  | <span data-ttu-id="2c03d-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c03d-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c03d-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-134">Request body</span></span>
<span data-ttu-id="2c03d-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c03d-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c03d-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2c03d-136">Parameter</span></span>      | <span data-ttu-id="2c03d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c03d-137">Type</span></span>    |<span data-ttu-id="2c03d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c03d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c03d-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="2c03d-139">transferTarget</span></span>|[<span data-ttu-id="2c03d-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="2c03d-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="2c03d-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="2c03d-141">The participant which is the target of the transfer.</span></span>|

## <a name="response"></a><span data-ttu-id="2c03d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c03d-142">Response</span></span>
<span data-ttu-id="2c03d-143">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="2c03d-143">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2c03d-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c03d-144">Examples</span></span>
<span data-ttu-id="2c03d-145">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="2c03d-145">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="2c03d-146">Exemplo 1: transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="2c03d-146">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="2c03d-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-147">Request</span></span>
<span data-ttu-id="2c03d-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c03d-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c03d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c03d-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c03d-150">C#</span><span class="sxs-lookup"><span data-stu-id="2c03d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c03d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c03d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c03d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c03d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c03d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c03d-153">Response</span></span>

> <span data-ttu-id="2c03d-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c03d-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2c03d-155">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-155">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2c03d-156">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="2c03d-156">Notification - transfer accepted</span></span>

> <span data-ttu-id="2c03d-157">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="2c03d-157">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2c03d-158">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="2c03d-158">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="2c03d-159">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-159">Notification - transfer failed</span></span>

> <span data-ttu-id="2c03d-160">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="2c03d-160">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="2c03d-161">Exemplo 2: transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="2c03d-161">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="2c03d-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-162">Request</span></span>
<span data-ttu-id="2c03d-163">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c03d-163">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c03d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c03d-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c03d-165">C#</span><span class="sxs-lookup"><span data-stu-id="2c03d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c03d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c03d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c03d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c03d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c03d-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c03d-168">Response</span></span>

> <span data-ttu-id="2c03d-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c03d-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2c03d-170">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-170">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2c03d-171">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="2c03d-171">Notification - transfer accepted</span></span>

> <span data-ttu-id="2c03d-172">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="2c03d-172">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2c03d-173">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="2c03d-173">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="2c03d-174">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-174">Notification - transfer failed</span></span>

> <span data-ttu-id="2c03d-175">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="2c03d-175">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="2c03d-176">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="2c03d-176">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="2c03d-177">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="2c03d-177">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="2c03d-178">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="2c03d-178">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="2c03d-179">**Observação:** Telefone ID é o número de telefone no formato E.164.</span><span class="sxs-lookup"><span data-stu-id="2c03d-179">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="2c03d-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-180">Request</span></span>
<span data-ttu-id="2c03d-181">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c03d-181">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c03d-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c03d-182">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c03d-183">C#</span><span class="sxs-lookup"><span data-stu-id="2c03d-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c03d-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c03d-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c03d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c03d-185">Response</span></span>

> <span data-ttu-id="2c03d-186">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c03d-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2c03d-187">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-187">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2c03d-188">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="2c03d-188">Notification - transfer accepted</span></span>

> <span data-ttu-id="2c03d-189">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="2c03d-189">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2c03d-190">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="2c03d-190">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="2c03d-191">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-191">Notification - transfer failed</span></span>

> <span data-ttu-id="2c03d-192">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="2c03d-192">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="2c03d-193">Exemplo 4: transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="2c03d-193">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="2c03d-194">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="2c03d-194">This call requires an application instance with a PSTN number assigned.</span></span> <span data-ttu-id="2c03d-195">Para obter detalhes, [consulte Atribuir um número de telefone ao seu bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span><span class="sxs-lookup"><span data-stu-id="2c03d-195">For details, see [Assign a phone number to your bot](/graph/cloud-communications-phone-number#assign-a-phone-number-to-your-bot).</span></span>
> <span data-ttu-id="2c03d-196">**Observação:** Telefone ID é o número de telefone no formato E.164.</span><span class="sxs-lookup"><span data-stu-id="2c03d-196">**Note:** Phone ID is the phone number in E.164 format.</span></span>

#### <a name="request"></a><span data-ttu-id="2c03d-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c03d-197">Request</span></span>
<span data-ttu-id="2c03d-198">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c03d-198">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c03d-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c03d-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c03d-200">C#</span><span class="sxs-lookup"><span data-stu-id="2c03d-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c03d-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c03d-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c03d-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c03d-202">Response</span></span>

> <span data-ttu-id="2c03d-203">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c03d-203">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="2c03d-204">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-204">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="2c03d-205">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="2c03d-205">Notification - transfer accepted</span></span>

> <span data-ttu-id="2c03d-206">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado de mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="2c03d-206">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="2c03d-207">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="2c03d-207">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="2c03d-208">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="2c03d-208">Notification - transfer failed</span></span>

> <span data-ttu-id="2c03d-209">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="2c03d-209">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


