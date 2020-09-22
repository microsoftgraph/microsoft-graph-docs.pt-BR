---
title: Obter o status de comando do dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa de códigos de status, confira lista de actionStatus.
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: 96098db1cf0e630c46a838b7712141ea4182779e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991212"
---
# <a name="get-device-command-status"></a><span data-ttu-id="f05f4-104">Obter o status de comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f05f4-104">Get device command status</span></span>

<span data-ttu-id="f05f4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f05f4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05f4-106">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f05f4-106">Get the status of a command on a device.</span></span> <span data-ttu-id="f05f4-107">Para obter a lista completa de códigos de status, confira [lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="f05f4-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="f05f4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f05f4-108">Permissions</span></span>

<span data-ttu-id="f05f4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f05f4-111">Permission type</span></span>      | <span data-ttu-id="f05f4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f05f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f05f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f05f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f05f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f4-114">Not supported.</span></span>    |
|<span data-ttu-id="f05f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f05f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f05f4-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f05f4-116">Device.Command</span></span>    |
|<span data-ttu-id="f05f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f05f4-117">Application</span></span> | <span data-ttu-id="f05f4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f05f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f05f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f05f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f4-120">Request headers</span></span>

| <span data-ttu-id="f05f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f05f4-121">Header</span></span> |<span data-ttu-id="f05f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f05f4-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="f05f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f05f4-123">Authorization</span></span>| <span data-ttu-id="f05f4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05f4-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f05f4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f05f4-126">Accept</span></span> | <span data-ttu-id="f05f4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f05f4-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="f05f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f4-128">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a><span data-ttu-id="f05f4-129">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="f05f4-129">List of actionStatus</span></span>

- <span data-ttu-id="f05f4-130">a solicitação,//comando foi criada e está aguardando processamento</span><span class="sxs-lookup"><span data-stu-id="f05f4-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="f05f4-131">o comando sentToTarget,//foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="f05f4-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="f05f4-132">executando,//dispositivo de destino confirmado o recebimento do comando e o está executando</span><span class="sxs-lookup"><span data-stu-id="f05f4-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="f05f4-133">conclusão da execução do comando//concluída</span><span class="sxs-lookup"><span data-stu-id="f05f4-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="f05f4-134">failedToSend,//Service falhou ao enviar comando para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="f05f4-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="f05f4-135">falha na execução do comando executionFailed,//</span><span class="sxs-lookup"><span data-stu-id="f05f4-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="f05f4-136">commandDropped,//comando Descartado pelo cliente se o dispositivo estiver no estado ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="f05f4-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="f05f4-137">cancelar,//cancelar o comando</span><span class="sxs-lookup"><span data-stu-id="f05f4-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="f05f4-138">Cancelando,//cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="f05f4-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="f05f4-139">o comando cancelado,//foi cancelado</span><span class="sxs-lookup"><span data-stu-id="f05f4-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="f05f4-140">repetir,//o serviço está tentando enviar novamente o comando para o destino</span><span class="sxs-lookup"><span data-stu-id="f05f4-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="f05f4-141">expirado,//o processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="f05f4-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="f05f4-142">erro,//erro interno ao processar o comando</span><span class="sxs-lookup"><span data-stu-id="f05f4-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="f05f4-143">status personalizado//personalizado</span><span class="sxs-lookup"><span data-stu-id="f05f4-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="f05f4-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f05f4-144">Example</span></span>

<span data-ttu-id="f05f4-145">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f05f4-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f05f4-146">A ID do dispositivo é retornada ao emitir uma chamada GET para `/me/devices` , e a ID do comando é retornada ao realizar uma chamada post em `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="f05f4-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f05f4-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f4-147">Request</span></span>

<span data-ttu-id="f05f4-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f05f4-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f05f4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f4-149">Response</span></span>

<span data-ttu-id="f05f4-150">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f05f4-150">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a><span data-ttu-id="f05f4-151">Obter conteúdo do comando</span><span class="sxs-lookup"><span data-stu-id="f05f4-151">Get command payload</span></span>

<span data-ttu-id="f05f4-152">Obter uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f05f4-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="f05f4-153">A carga de resposta é usada ao consultar um serviço de aplicativo para transportar dados de volta.</span><span class="sxs-lookup"><span data-stu-id="f05f4-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="f05f4-154">Permissões</span><span class="sxs-lookup"><span data-stu-id="f05f4-154">Permissions</span></span>

<span data-ttu-id="f05f4-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05f4-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05f4-157">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f05f4-157">Permission type</span></span>      | <span data-ttu-id="f05f4-158">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f05f4-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f05f4-159">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f05f4-159">Delegated (work or school account)</span></span> | <span data-ttu-id="f05f4-160">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f4-160">Not supported.</span></span>    |
|<span data-ttu-id="f05f4-161">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f05f4-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f05f4-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f05f4-162">Device.Command</span></span>    |
|<span data-ttu-id="f05f4-163">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f05f4-163">Application</span></span> | <span data-ttu-id="f05f4-164">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f4-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="f05f4-165">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f05f4-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="f05f4-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f4-166">Request headers</span></span>

| <span data-ttu-id="f05f4-167">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f05f4-167">Header</span></span> |<span data-ttu-id="f05f4-168">Valor</span><span class="sxs-lookup"><span data-stu-id="f05f4-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="f05f4-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="f05f4-169">Authorization</span></span>| <span data-ttu-id="f05f4-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05f4-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f05f4-172">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f05f4-172">Accept</span></span> | <span data-ttu-id="f05f4-173">application/json</span><span class="sxs-lookup"><span data-stu-id="f05f4-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="f05f4-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f4-174">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a><span data-ttu-id="f05f4-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f05f4-175">Example</span></span>

<span data-ttu-id="f05f4-176">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f05f4-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f05f4-177">A ID do dispositivo é retornada ao emitir uma chamada GET em `/me/devices` e a ID do comando é retornada ao executar uma chamada post em `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="f05f4-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f05f4-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f4-178">Request</span></span>

<span data-ttu-id="f05f4-179">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f05f4-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f05f4-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f4-180">Response</span></span>

<span data-ttu-id="f05f4-181">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="f05f4-181">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```


