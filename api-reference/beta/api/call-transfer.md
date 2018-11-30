---
title: 'chamar: transferência'
description: Transferir uma chamada ativa.
ms.openlocfilehash: d02e028c4d7e3b51f3aee371e22d00b95841d9a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037778"
---
# <a name="call-transfer"></a><span data-ttu-id="613b9-103">chamar: transferência</span><span class="sxs-lookup"><span data-stu-id="613b9-103">call: transfer</span></span>

> <span data-ttu-id="613b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="613b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="613b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="613b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="613b9-106">Transferir uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="613b9-106">Transfer an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="613b9-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="613b9-107">Permissions</span></span>
<span data-ttu-id="613b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="613b9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="613b9-110">Permission type</span></span> | <span data-ttu-id="613b9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="613b9-111">Permissions (from least to most privileged)</span></span>         |
| :-------------- | :-------------------------------------------------- |
| <span data-ttu-id="613b9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="613b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="613b9-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="613b9-113">Not Supported</span></span>                |
| <span data-ttu-id="613b9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="613b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613b9-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="613b9-115">Not Supported</span></span>                |
| <span data-ttu-id="613b9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="613b9-116">Application</span></span>     | <span data-ttu-id="613b9-117">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="613b9-117">Calls.Initiate.All</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="613b9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="613b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/transfer
POST /applications/{id}/calls/{id}/transfer
```

## <a name="request-headers"></a><span data-ttu-id="613b9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="613b9-119">Request headers</span></span>
| <span data-ttu-id="613b9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="613b9-120">Name</span></span>          | <span data-ttu-id="613b9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="613b9-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="613b9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="613b9-122">Authorization</span></span> | <span data-ttu-id="613b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="613b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="613b9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="613b9-125">Request body</span></span>
<span data-ttu-id="613b9-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="613b9-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="613b9-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="613b9-127">Parameter</span></span>      | <span data-ttu-id="613b9-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="613b9-128">Type</span></span>    |<span data-ttu-id="613b9-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="613b9-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="613b9-130">transferTarget</span><span class="sxs-lookup"><span data-stu-id="613b9-130">transferTarget</span></span>|[<span data-ttu-id="613b9-131">invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="613b9-131">invitationParticipantInfo</span></span>](../resources/invitationparticipantinfo.md)|<span data-ttu-id="613b9-132">O participante que é o destino da transferência.</span><span class="sxs-lookup"><span data-stu-id="613b9-132">The participant which is the target of the transfer.</span></span>|
|<span data-ttu-id="613b9-133">destino</span><span class="sxs-lookup"><span data-stu-id="613b9-133">target</span></span>|[<span data-ttu-id="613b9-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="613b9-134">identitySet</span></span>](../resources/identityset.md)||
|<span data-ttu-id="613b9-135">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="613b9-135">replacesCallId</span></span>|<span data-ttu-id="613b9-136">String</span><span class="sxs-lookup"><span data-stu-id="613b9-136">String</span></span>|<span data-ttu-id="613b9-137">Id de chamada original do participante que está sendo transferido.</span><span class="sxs-lookup"><span data-stu-id="613b9-137">Original call id of the participant that is being transferred.</span></span>|
|<span data-ttu-id="613b9-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="613b9-138">clientContext</span></span>|<span data-ttu-id="613b9-139">String</span><span class="sxs-lookup"><span data-stu-id="613b9-139">String</span></span>|<span data-ttu-id="613b9-140">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="613b9-140">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="613b9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="613b9-141">Response</span></span>
<span data-ttu-id="613b9-142">Retorna `202 Accepted` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="613b9-142">Returns `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="613b9-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="613b9-143">Examples</span></span>

### <a name="transfer-call-directly-with-no-user-involvement"></a><span data-ttu-id="613b9-144">Transferir a chamada diretamente, com nenhum envolvimento do usuário</span><span class="sxs-lookup"><span data-stu-id="613b9-144">Transfer call directly, with no user involvement</span></span>

<span data-ttu-id="613b9-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="613b9-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="613b9-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="613b9-146">Request</span></span>
<span data-ttu-id="613b9-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="613b9-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call_transfer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/transfer
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
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="613b9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="613b9-148">Response</span></span>

> <span data-ttu-id="613b9-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="613b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
}-->
```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="613b9-151">Notificação - transferindo</span><span class="sxs-lookup"><span data-stu-id="613b9-151">Notification - transferring</span></span>

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
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="613b9-152">Notificação - transferência aceito</span><span class="sxs-lookup"><span data-stu-id="613b9-152">Notification - transfer accepted</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="613b9-153">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="613b9-153">Notification - terminated</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

### <a name="consultative-transfer"></a><span data-ttu-id="613b9-154">Transferência com consultoria</span><span class="sxs-lookup"><span data-stu-id="613b9-154">Consultative transfer</span></span>

##### <a name="request"></a><span data-ttu-id="613b9-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="613b9-155">Request</span></span>

```http
POST /app/calls/57DAB8B1894C409AB240BD8BEAE78896/transfer
Authorization: Bearer <TOKEN>
Content-Type: application/json
```
<!-- {
  "blockType": "ignored",
  "@odata.type": "call_transfer"
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "transferTarget": {
    "endpointType": "default",
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus",
    "replacesCallId": "e5d39592-99bd-4db8-bca8-30fb894ec51d"
  }
}
```

##### <a name="response"></a><span data-ttu-id="613b9-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="613b9-156">Response</span></span>

> <span data-ttu-id="613b9-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="613b9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 202 Accepted
```

##### <a name="notification---transferring"></a><span data-ttu-id="613b9-159">Notificação - transferindo</span><span class="sxs-lookup"><span data-stu-id="613b9-159">Notification - transferring</span></span>

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
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferring"
        },
        "status": "running"
      }
    }
  ]
}
```

##### <a name="notification---transfer-accepted"></a><span data-ttu-id="613b9-160">Notificação - transferência aceito</span><span class="sxs-lookup"><span data-stu-id="613b9-160">Notification - transfer accepted</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "resultInfo": {
          "code": "200",
          "subCode": "transferAccepted"
        },
        "status": "completed"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="613b9-161">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="613b9-161">Notification - terminated</span></span>

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
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppTransferred"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: transfer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
