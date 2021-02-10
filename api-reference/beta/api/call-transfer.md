---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 1d7f38e5fc128d176ff5c954ae0dae7113f18285
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176579"
---
# <a name="call-transfer"></a><span data-ttu-id="d3843-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="d3843-103">call: transfer</span></span>

<span data-ttu-id="d3843-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3843-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3843-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="d3843-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="d3843-106">**Observação:** Isso só será suportado se os destinos de transferência e transferência são usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="d3843-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="d3843-107">A transferência para o número PSTN é suportada apenas para a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-107">Transfer to PSTN number is supported only for application instance.</span></span> <span data-ttu-id="d3843-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="d3843-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="d3843-109">Uma transferência consultiva significa que o transferor pode informar a pessoa para a quem ele deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="d3843-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="d3843-110">Isso não é transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="d3843-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3843-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3843-111">Permissions</span></span>
<span data-ttu-id="d3843-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3843-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3843-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3843-114">Permission type</span></span> | <span data-ttu-id="d3843-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3843-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="d3843-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3843-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3843-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d3843-117">Not Supported</span></span>                |
| <span data-ttu-id="d3843-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3843-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3843-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="d3843-119">Not Supported</span></span>                |
| <span data-ttu-id="d3843-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3843-120">Application</span></span>     | <span data-ttu-id="d3843-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="d3843-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="d3843-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3843-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /communications/calls/{id}/transfer
```
> <span data-ttu-id="d3843-123">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="d3843-123">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="d3843-124">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="d3843-124">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3843-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-125">Request headers</span></span>
| <span data-ttu-id="d3843-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d3843-126">Name</span></span>          | <span data-ttu-id="d3843-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3843-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d3843-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3843-128">Authorization</span></span> | <span data-ttu-id="d3843-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3843-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3843-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="d3843-131">Content-type</span></span>  | <span data-ttu-id="d3843-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3843-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3843-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-134">Request body</span></span>
<span data-ttu-id="d3843-135">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3843-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3843-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3843-136">Parameter</span></span>      | <span data-ttu-id="d3843-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3843-137">Type</span></span>    |<span data-ttu-id="d3843-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3843-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3843-139">transferTarget</span><span class="sxs-lookup"><span data-stu-id="d3843-139">transferTarget</span></span>|[<span data-ttu-id="d3843-140">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="d3843-140">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="d3843-141">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="d3843-141">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="d3843-142">clientContext</span><span class="sxs-lookup"><span data-stu-id="d3843-142">clientContext</span></span>|<span data-ttu-id="d3843-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3843-143">String</span></span>|<span data-ttu-id="d3843-144">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="d3843-144">Unique Client Context string.</span></span> <span data-ttu-id="d3843-145">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d3843-145">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="d3843-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3843-146">Response</span></span>
<span data-ttu-id="d3843-147">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d3843-147">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d3843-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3843-148">Examples</span></span>
<span data-ttu-id="d3843-149">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="d3843-149">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="d3843-150">Exemplo 1: Transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="d3843-150">Example 1: Call transfer</span></span>

#### <a name="request"></a><span data-ttu-id="d3843-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-151">Request</span></span>
<span data-ttu-id="d3843-152">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3843-152">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3843-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3843-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3843-154">C#</span><span class="sxs-lookup"><span data-stu-id="d3843-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3843-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3843-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3843-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3843-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d3843-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3843-157">Response</span></span>

> <span data-ttu-id="d3843-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3843-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d3843-160">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-160">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d3843-161">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="d3843-161">Notification - transfer accepted</span></span>

> <span data-ttu-id="d3843-162">**Observação:** A transferência aceita pode acontecer após ou antes do estado de mídia de áudio inativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-162">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d3843-163">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="d3843-163">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="d3843-164">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-164">Notification - transfer failed</span></span>

> <span data-ttu-id="d3843-165">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="d3843-165">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="d3843-166">Exemplo 2: Transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="d3843-166">Example 2: Consultative transfer</span></span>

#### <a name="request"></a><span data-ttu-id="d3843-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-167">Request</span></span>
<span data-ttu-id="d3843-168">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3843-168">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d3843-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3843-169">Response</span></span>

> <span data-ttu-id="d3843-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3843-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d3843-172">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-172">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d3843-173">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="d3843-173">Notification - transfer accepted</span></span>

> <span data-ttu-id="d3843-174">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-174">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d3843-175">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="d3843-175">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="d3843-176">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-176">Notification - transfer failed</span></span>

> <span data-ttu-id="d3843-177">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="d3843-177">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="d3843-178">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="d3843-178">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="d3843-179">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="d3843-179">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="d3843-180">Etapa 1: Criar instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3843-180">Step 1: Create application instance</span></span>
<span data-ttu-id="d3843-181">Usando credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para criar a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-181">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="d3843-182">Para obter mais informações, [consulte New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d3843-182">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="d3843-183">Etapa 2: Atribuir licenças do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d3843-183">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="d3843-184">Use as credenciais de administrador de locatários para entrar e acessar a guia https://admin.microsoft.com/ **Usuários -> Usuários ativos.**</span><span class="sxs-lookup"><span data-stu-id="d3843-184">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="d3843-185">Selecione a instância do aplicativo, atribua o Plano de Chamadas Domésticas e Internacionais do **Microsoft 365** e o Sistema de Telefonia do **Microsoft 365 -** Licenças de Usuário Virtual e clique em Salvar **alterações.**</span><span class="sxs-lookup"><span data-stu-id="d3843-185">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="d3843-186">Se as licenças necessárias não estão disponíveis no locatário, você pode obter-as na guia Cobrança **-> serviços de** compra.</span><span class="sxs-lookup"><span data-stu-id="d3843-186">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="d3843-187">Etapa 3: Adquirir número PSTN</span><span class="sxs-lookup"><span data-stu-id="d3843-187">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="d3843-188">Use as credenciais de administrador de locatários para entrar e clique na guia https://admin.teams.microsoft.com/ **Portal** herddo no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="d3843-188">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="d3843-189">Na nova página, vá para a **guia de números de telefone > voz.**</span><span class="sxs-lookup"><span data-stu-id="d3843-189">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="d3843-190">Clique no botão, selecione Novos Números de Serviço e vá para a página Adicionar **+** **novos números de** serviço. </span><span class="sxs-lookup"><span data-stu-id="d3843-190">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="d3843-191">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span><span class="sxs-lookup"><span data-stu-id="d3843-191">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="d3843-192">Clique **em adquirir números.**</span><span class="sxs-lookup"><span data-stu-id="d3843-192">Click **acquire numbers**.</span></span> <span data-ttu-id="d3843-193">O número recém-adquirido será aparecer na guia **números de** telefone.</span><span class="sxs-lookup"><span data-stu-id="d3843-193">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="d3843-194">Etapa 4: Atribuir número PSTN à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3843-194">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="d3843-195">Com credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para atribuir o número PSTN à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-195">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="d3843-196">Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d3843-196">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="d3843-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-197">Request</span></span>
<span data-ttu-id="d3843-198">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3843-198">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d3843-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3843-199">Response</span></span>

> <span data-ttu-id="d3843-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3843-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d3843-202">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-202">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d3843-203">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="d3843-203">Notification - transfer accepted</span></span>

> <span data-ttu-id="d3843-204">**Observação:** A transferência aceita pode acontecer após ou antes do estado de mídia de áudio inativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-204">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d3843-205">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="d3843-205">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="d3843-206">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-206">Notification - transfer failed</span></span>

> <span data-ttu-id="d3843-207">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="d3843-207">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="d3843-208">Exemplo 4: Transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="d3843-208">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="d3843-209">Essa chamada requer uma instância de aplicativo com o número PSTN atribuído, conforme descrito no Exemplo 3.</span><span class="sxs-lookup"><span data-stu-id="d3843-209">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

#### <a name="request"></a><span data-ttu-id="d3843-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3843-210">Request</span></span>
<span data-ttu-id="d3843-211">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3843-211">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d3843-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3843-212">Response</span></span>

> <span data-ttu-id="d3843-p115">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3843-p115">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="d3843-215">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-215">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="d3843-216">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="d3843-216">Notification - transfer accepted</span></span>

> <span data-ttu-id="d3843-217">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="d3843-217">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="d3843-218">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="d3843-218">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="d3843-219">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="d3843-219">Notification - transfer failed</span></span>

> <span data-ttu-id="d3843-220">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="d3843-220">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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


