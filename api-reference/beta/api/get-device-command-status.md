---
title: Obter o status de comando do dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa de códigos de status, confira lista de actionStatus.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: fee9b291145bce2e5cca4bc54405a833e95ec053
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421435"
---
# <a name="get-device-command-status"></a><span data-ttu-id="b6f77-104">Obter o status de comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b6f77-104">Get device command status</span></span>

<span data-ttu-id="b6f77-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6f77-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6f77-106">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6f77-106">Get the status of a command on a device.</span></span> <span data-ttu-id="b6f77-107">Para obter a lista completa de códigos de status, confira [lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="b6f77-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6f77-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6f77-108">Permissions</span></span>

<span data-ttu-id="b6f77-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f77-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f77-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f77-111">Permission type</span></span>      | <span data-ttu-id="b6f77-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6f77-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f77-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f77-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f77-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f77-114">Not supported.</span></span>    |
|<span data-ttu-id="b6f77-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f77-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f77-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="b6f77-116">Device.Command</span></span>    |
|<span data-ttu-id="b6f77-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f77-117">Application</span></span> | <span data-ttu-id="b6f77-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f77-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6f77-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f77-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b6f77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f77-120">Request headers</span></span>

| <span data-ttu-id="b6f77-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f77-121">Header</span></span> |<span data-ttu-id="b6f77-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f77-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="b6f77-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f77-123">Authorization</span></span>| <span data-ttu-id="b6f77-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f77-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b6f77-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6f77-126">Accept</span></span> | <span data-ttu-id="b6f77-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f77-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="b6f77-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f77-128">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="b6f77-129">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="b6f77-129">List of actionStatus</span></span>

- <span data-ttu-id="b6f77-130">a solicitação,//comando foi criada e está aguardando processamento</span><span class="sxs-lookup"><span data-stu-id="b6f77-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="b6f77-131">o comando sentToTarget,//foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="b6f77-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="b6f77-132">executando,//dispositivo de destino confirmado o recebimento do comando e o está executando</span><span class="sxs-lookup"><span data-stu-id="b6f77-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="b6f77-133">conclusão da execução do comando//concluída</span><span class="sxs-lookup"><span data-stu-id="b6f77-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="b6f77-134">failedToSend,//Service falhou ao enviar comando para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="b6f77-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="b6f77-135">falha na execução do comando executionFailed,//</span><span class="sxs-lookup"><span data-stu-id="b6f77-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="b6f77-136">commandDropped,//comando Descartado pelo cliente se o dispositivo estiver no estado ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="b6f77-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="b6f77-137">cancelar,//cancelar o comando</span><span class="sxs-lookup"><span data-stu-id="b6f77-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="b6f77-138">Cancelando,//cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="b6f77-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="b6f77-139">o comando cancelado,//foi cancelado</span><span class="sxs-lookup"><span data-stu-id="b6f77-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="b6f77-140">repetir,//o serviço está tentando enviar novamente o comando para o destino</span><span class="sxs-lookup"><span data-stu-id="b6f77-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="b6f77-141">expirado,//o processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="b6f77-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="b6f77-142">erro,//erro interno ao processar o comando</span><span class="sxs-lookup"><span data-stu-id="b6f77-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="b6f77-143">status personalizado//personalizado</span><span class="sxs-lookup"><span data-stu-id="b6f77-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="b6f77-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f77-144">Example</span></span>

<span data-ttu-id="b6f77-145">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6f77-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="b6f77-146">A ID do dispositivo é retornada ao emitir uma chamada GET para `/me/devices`, e a ID do comando é retornada ao realizar uma chamada post `/me/devices/{id}/command`em.</span><span class="sxs-lookup"><span data-stu-id="b6f77-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="b6f77-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f77-147">Request</span></span>

<span data-ttu-id="b6f77-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f77-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="b6f77-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f77-149">Response</span></span>

<span data-ttu-id="b6f77-150">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f77-150">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="b6f77-151">Obter conteúdo do comando</span><span class="sxs-lookup"><span data-stu-id="b6f77-151">Get command payload</span></span>

<span data-ttu-id="b6f77-152">Obter uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6f77-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="b6f77-153">A carga de resposta é usada ao consultar um serviço de aplicativo para transportar dados de volta.</span><span class="sxs-lookup"><span data-stu-id="b6f77-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="b6f77-154">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6f77-154">Permissions</span></span>

<span data-ttu-id="b6f77-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f77-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f77-157">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f77-157">Permission type</span></span>      | <span data-ttu-id="b6f77-158">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6f77-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6f77-159">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f77-159">Delegated (work or school account)</span></span> | <span data-ttu-id="b6f77-160">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f77-160">Not supported.</span></span>    |
|<span data-ttu-id="b6f77-161">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f77-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6f77-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="b6f77-162">Device.Command</span></span>    |
|<span data-ttu-id="b6f77-163">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f77-163">Application</span></span> | <span data-ttu-id="b6f77-164">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f77-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="b6f77-165">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f77-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="b6f77-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f77-166">Request headers</span></span>

| <span data-ttu-id="b6f77-167">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f77-167">Header</span></span> |<span data-ttu-id="b6f77-168">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f77-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="b6f77-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f77-169">Authorization</span></span>| <span data-ttu-id="b6f77-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f77-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="b6f77-172">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6f77-172">Accept</span></span> | <span data-ttu-id="b6f77-173">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f77-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="b6f77-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f77-174">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="b6f77-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f77-175">Example</span></span>

<span data-ttu-id="b6f77-176">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6f77-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="b6f77-177">A ID do dispositivo é retornada ao emitir uma chamada GET em `/me/devices`e a ID do comando é retornada ao executar uma chamada post em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="b6f77-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="b6f77-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f77-178">Request</span></span>

<span data-ttu-id="b6f77-179">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f77-179">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="b6f77-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f77-180">Response</span></span>

<span data-ttu-id="b6f77-181">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f77-181">The following example shows the response.</span></span>

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
