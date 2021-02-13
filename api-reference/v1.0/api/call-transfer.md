---
title: 'call: transfer'
description: Transferir uma chamada ponto a ponto ativa.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b8186913aa54afc02266216666d82bce28568fc4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177232"
---
# <a name="call-transfer"></a><span data-ttu-id="81b96-103">call: transfer</span><span class="sxs-lookup"><span data-stu-id="81b96-103">call: transfer</span></span>

<span data-ttu-id="81b96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81b96-105">Transferir uma chamada ponto a ponto ativa.</span><span class="sxs-lookup"><span data-stu-id="81b96-105">Transfer an active peer-to-peer call.</span></span>

> <span data-ttu-id="81b96-106">**Observação:** Isso só será suportado se os destinos de transferência e transferência são usuários do Microsoft Teams que pertencem ao mesmo locatário.</span><span class="sxs-lookup"><span data-stu-id="81b96-106">**Note:** This is only supported if both the transferee and transfer target are Microsoft Teams users that belong to the same tenant.</span></span> <span data-ttu-id="81b96-107">A transferência para o número PSTN não é suportada.</span><span class="sxs-lookup"><span data-stu-id="81b96-107">Transfer to PSTN number is not supported.</span></span> <span data-ttu-id="81b96-108">Para saber mais sobre o destino de transferência, transferência e transferência, consulte [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span><span class="sxs-lookup"><span data-stu-id="81b96-108">To learn more about transferor, transferee and transfer target, see [RFC 5589](https://tools.ietf.org/html/rfc5589#section-2).</span></span>

<span data-ttu-id="81b96-109">Uma transferência consultiva significa que o transferor pode informar a pessoa para a quem ele deseja transferir a chamada (o transferidor), antes que a transferência seja feita.</span><span class="sxs-lookup"><span data-stu-id="81b96-109">A consultative transfer means that the transferor can inform the person they want to transfer the call to (the transferee), before the transfer is made.</span></span> <span data-ttu-id="81b96-110">Isso não é transferir a chamada diretamente.</span><span class="sxs-lookup"><span data-stu-id="81b96-110">This is opposed to transfering the call directly.</span></span>

## <a name="permissions"></a><span data-ttu-id="81b96-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="81b96-111">Permissions</span></span>
<span data-ttu-id="81b96-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81b96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81b96-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81b96-114">Permission type</span></span> | <span data-ttu-id="81b96-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81b96-115">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="81b96-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81b96-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="81b96-117">Não suportado</span><span class="sxs-lookup"><span data-stu-id="81b96-117">Not Supported</span></span>                |
| <span data-ttu-id="81b96-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81b96-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81b96-119">Não suportado</span><span class="sxs-lookup"><span data-stu-id="81b96-119">Not Supported</span></span>                |
| <span data-ttu-id="81b96-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b96-120">Application</span></span>     | <span data-ttu-id="81b96-121">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="81b96-121">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="81b96-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81b96-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="81b96-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-123">Request headers</span></span>
| <span data-ttu-id="81b96-124">Nome</span><span class="sxs-lookup"><span data-stu-id="81b96-124">Name</span></span>          | <span data-ttu-id="81b96-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b96-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="81b96-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="81b96-126">Authorization</span></span> | <span data-ttu-id="81b96-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b96-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81b96-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="81b96-129">Content-type</span></span>  | <span data-ttu-id="81b96-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b96-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81b96-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-132">Request body</span></span>
<span data-ttu-id="81b96-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b96-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81b96-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="81b96-134">Parameter</span></span>      | <span data-ttu-id="81b96-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b96-135">Type</span></span>    |<span data-ttu-id="81b96-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b96-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81b96-137">transferTarget</span><span class="sxs-lookup"><span data-stu-id="81b96-137">transferTarget</span></span>|[<span data-ttu-id="81b96-138">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="81b96-138">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="81b96-139">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="81b96-139">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="81b96-140">clientContext</span><span class="sxs-lookup"><span data-stu-id="81b96-140">clientContext</span></span>|<span data-ttu-id="81b96-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81b96-141">String</span></span>|<span data-ttu-id="81b96-142">Cadeia de caracteres de contexto de cliente exclusiva.</span><span class="sxs-lookup"><span data-stu-id="81b96-142">Unique Client Context string.</span></span> <span data-ttu-id="81b96-143">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="81b96-143">Max limit is 256 chars.</span></span>|

## <a name="response"></a><span data-ttu-id="81b96-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b96-144">Response</span></span>
<span data-ttu-id="81b96-145">Se tiver êxito, este método retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="81b96-145">If successful, this method returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="81b96-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81b96-146">Examples</span></span>
<span data-ttu-id="81b96-147">Esses exemplos mostram o fluxo de uma chamada de entrada até os diferentes tipos de notificações de transferência.</span><span class="sxs-lookup"><span data-stu-id="81b96-147">These examples show the flow of an incoming call all the way to the different types of transfer notifications.</span></span>

### <a name="example-1-call-transfer"></a><span data-ttu-id="81b96-148">Exemplo 1: Transferência de chamada</span><span class="sxs-lookup"><span data-stu-id="81b96-148">Example 1: Call transfer</span></span>

##### <a name="request"></a><span data-ttu-id="81b96-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-149">Request</span></span>
<span data-ttu-id="81b96-150">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b96-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81b96-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="81b96-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="81b96-152">C#</span><span class="sxs-lookup"><span data-stu-id="81b96-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-transfer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81b96-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81b96-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-transfer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81b96-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81b96-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-transfer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81b96-155">Java</span><span class="sxs-lookup"><span data-stu-id="81b96-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-transfer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81b96-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b96-156">Response</span></span>

> <span data-ttu-id="81b96-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81b96-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="81b96-159">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-159">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="81b96-160">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="81b96-160">Notification - transfer accepted</span></span>

> <span data-ttu-id="81b96-161">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-161">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="81b96-162">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="81b96-162">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="81b96-163">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-163">Notification - transfer failed</span></span>

> <span data-ttu-id="81b96-164">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="81b96-164">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-2-consultative-transfer"></a><span data-ttu-id="81b96-165">Exemplo 2: Transferência consultiva</span><span class="sxs-lookup"><span data-stu-id="81b96-165">Example 2: Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="81b96-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-166">Request</span></span>
<span data-ttu-id="81b96-167">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b96-167">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="81b96-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b96-168">Response</span></span>

> <span data-ttu-id="81b96-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81b96-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="81b96-171">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-171">Notification - transferring</span></span>

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

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="81b96-172">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="81b96-172">Notification - transfer accepted</span></span>

> <span data-ttu-id="81b96-173">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-173">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

##### <a name="notification---transfer-completed"></a><span data-ttu-id="81b96-174">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="81b96-174">Notification - transfer completed</span></span>

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

##### <a name="notification---transfer-failed"></a><span data-ttu-id="81b96-175">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-175">Notification - transfer failed</span></span>

> <span data-ttu-id="81b96-176">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="81b96-176">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-3-call-transfer-to-pstn-number"></a><span data-ttu-id="81b96-177">Exemplo 3: Transferência de chamada para número PSTN</span><span class="sxs-lookup"><span data-stu-id="81b96-177">Example 3: Call transfer to PSTN number</span></span>

<span data-ttu-id="81b96-178">Essa chamada requer uma instância de aplicativo com um número PSTN atribuído.</span><span class="sxs-lookup"><span data-stu-id="81b96-178">This call requires an application instance with a PSTN number assigned.</span></span>

#### <a name="step-1-create-application-instance"></a><span data-ttu-id="81b96-179">Etapa 1: Criar instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b96-179">Step 1: Create application instance</span></span>
<span data-ttu-id="81b96-180">Usando credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para criar a instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-180">Using tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to create the application instance.</span></span> <span data-ttu-id="81b96-181">Para obter mais informações, [consulte New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="81b96-181">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <UPN> -DisplayName <DisplayName> -ApplicationId <AppId>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```
#### <a name="step-2-assign-microsoft-365-licenses"></a><span data-ttu-id="81b96-182">Etapa 2: Atribuir licenças do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="81b96-182">Step 2: Assign Microsoft 365 licenses</span></span>
1. <span data-ttu-id="81b96-183">Use as credenciais de administrador de locatários para entrar e acessar a guia https://admin.microsoft.com/ **Usuários -> Usuários ativos.**</span><span class="sxs-lookup"><span data-stu-id="81b96-183">Use tenant admin credentials to sign in to https://admin.microsoft.com/ and go to the **Users -> Active users** tab.</span></span>
2. <span data-ttu-id="81b96-184">Selecione a instância do aplicativo, atribua o Plano de Chamadas Domésticas e Internacionais do **Microsoft 365** e o Sistema de Telefonia do **Microsoft 365 -** Licenças de Usuário Virtual e clique em Salvar **alterações.**</span><span class="sxs-lookup"><span data-stu-id="81b96-184">Select the application instance, assign **Microsoft 365 Domestic and International Calling Plan** and **Microsoft 365 Phone System - Virtual User** licenses, and click **Save changes**.</span></span> <span data-ttu-id="81b96-185">Se as licenças necessárias não estão disponíveis no locatário, você pode obter-as na guia Cobrança **-> serviços de** compra.</span><span class="sxs-lookup"><span data-stu-id="81b96-185">If the required licenses are not available in the tenant, you can get them from the **Billing -> Purchase services** tab.</span></span>
#### <a name="step-3-acquire-pstn-number"></a><span data-ttu-id="81b96-186">Etapa 3: Adquirir número PSTN</span><span class="sxs-lookup"><span data-stu-id="81b96-186">Step 3: Acquire PSTN number</span></span>
1. <span data-ttu-id="81b96-187">Use as credenciais de administrador de locatários para entrar e clique na guia https://admin.teams.microsoft.com/ **Portal** herddo no painel esquerdo.</span><span class="sxs-lookup"><span data-stu-id="81b96-187">Use tenant admin credentials to sign in to https://admin.teams.microsoft.com/ and click the **Legacy portal** tab on the left panel.</span></span>
2. <span data-ttu-id="81b96-188">Na nova página, vá para a **guia de números de telefone > voz.**</span><span class="sxs-lookup"><span data-stu-id="81b96-188">In the new page, go to the **voice -> phone numbers** tab.</span></span>
3. <span data-ttu-id="81b96-189">Clique no botão, selecione Novos Números de Serviço e vá para a página Adicionar **+** **novos números de** serviço. </span><span class="sxs-lookup"><span data-stu-id="81b96-189">Click the **+** button, select **New Service Numbers**, and go to the **Add new service numbers** page.</span></span>
4. <span data-ttu-id="81b96-190">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span><span class="sxs-lookup"><span data-stu-id="81b96-190">Select **Country/Region**, **State/Region**, **City**, input **Quantity**, and click **add** to search.</span></span> <span data-ttu-id="81b96-191">Clique **em adquirir números.**</span><span class="sxs-lookup"><span data-stu-id="81b96-191">Click **acquire numbers**.</span></span> <span data-ttu-id="81b96-192">O número recém-adquirido será aparecer na guia **números de** telefone.</span><span class="sxs-lookup"><span data-stu-id="81b96-192">The newly acquired number will show on  the **phone numbers** tab.</span></span>
#### <a name="step-4-assign-pstn-number-to-application-instance"></a><span data-ttu-id="81b96-193">Etapa 4: Atribuir número PSTN à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b96-193">Step 4: Assign PSTN number to application instance</span></span>
<span data-ttu-id="81b96-194">Com credenciais de administrador de locatários, chame os cmdlets a seguir no PowerShell remoto do locatário para atribuir o número PSTN à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-194">With tenant admin credentials, call the following cmdlets on the tenant remote PowerShell to assign the PSTN number to the application instance.</span></span> <span data-ttu-id="81b96-195">Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="81b96-195">For more information, see [Set-CsOnlineVoiceApplicationInstance](https://docs.microsoft.com/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](https://docs.microsoft.com/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>
```
PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <UPN> -TelephoneNumber <TelephoneNumber>
PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <ObjectId>
```

#### <a name="request"></a><span data-ttu-id="81b96-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-196">Request</span></span>
<span data-ttu-id="81b96-197">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b96-197">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="81b96-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b96-198">Response</span></span>

> <span data-ttu-id="81b96-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81b96-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="81b96-201">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-201">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="81b96-202">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="81b96-202">Notification - transfer accepted</span></span>

> <span data-ttu-id="81b96-203">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-203">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="81b96-204">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="81b96-204">Notification - transfer completed</span></span>

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
### <a name="notification---transfer-failed"></a><span data-ttu-id="81b96-205">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-205">Notification - transfer failed</span></span>

> <span data-ttu-id="81b96-206">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="81b96-206">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

### <a name="example-4-consultative-transfer-to-pstn-number"></a><span data-ttu-id="81b96-207">Exemplo 4: Transferência consultiva para número PSTN</span><span class="sxs-lookup"><span data-stu-id="81b96-207">Example 4: Consultative transfer to PSTN number</span></span>

<span data-ttu-id="81b96-208">Essa chamada requer uma instância de aplicativo com o número PSTN atribuído, conforme descrito no Exemplo 3.</span><span class="sxs-lookup"><span data-stu-id="81b96-208">This call requires an application instance with PSTN number assigned, as described in Example 3.</span></span>

#### <a name="request"></a><span data-ttu-id="81b96-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b96-209">Request</span></span>
<span data-ttu-id="81b96-210">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b96-210">The following example shows the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="81b96-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b96-211">Response</span></span>

> <span data-ttu-id="81b96-p114">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81b96-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

#### <a name="notification---transferring"></a><span data-ttu-id="81b96-214">Notificação - transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-214">Notification - transferring</span></span>

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

#### <a name="notification---transfer-accepted"></a><span data-ttu-id="81b96-215">Notificação - transferência aceita</span><span class="sxs-lookup"><span data-stu-id="81b96-215">Notification - transfer accepted</span></span>

> <span data-ttu-id="81b96-216">**Observação:** A transferência aceita pode acontecer após ou antes que o áudio do estado da mídia seja inativo.</span><span class="sxs-lookup"><span data-stu-id="81b96-216">**Note:** Transfer accepted may happen after or before media state audio inactive.</span></span>

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

#### <a name="notification---transfer-completed"></a><span data-ttu-id="81b96-217">Notificação - transferência concluída</span><span class="sxs-lookup"><span data-stu-id="81b96-217">Notification - transfer completed</span></span>

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

#### <a name="notification---transfer-failed"></a><span data-ttu-id="81b96-218">Notificação - falha na transferência</span><span class="sxs-lookup"><span data-stu-id="81b96-218">Notification - transfer failed</span></span>

> <span data-ttu-id="81b96-219">**Observação:** Quando uma transferência de chamada falhar, o estado da chamada será `established` .</span><span class="sxs-lookup"><span data-stu-id="81b96-219">**Note:** When a call transfer fails, the call state will be `established`.</span></span>

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

