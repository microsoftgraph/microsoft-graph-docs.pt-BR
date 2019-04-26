---
title: Obter o status de comando do dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa de códigos de status, confira lista de actionStatus.
localization_priority: Normal
ms.openlocfilehash: 9b914cdfde78ce50df812acb09dc034c978c7e08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324987"
---
# <a name="get-device-command-status"></a><span data-ttu-id="fdec6-104">Obter o status de comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fdec6-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdec6-105">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdec6-105">Get the status of a command on a device.</span></span> <span data-ttu-id="fdec6-106">Para obter a lista completa de códigos de status, confira [lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="fdec6-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="fdec6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdec6-107">Permissions</span></span>

<span data-ttu-id="fdec6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdec6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdec6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdec6-110">Permission type</span></span>      | <span data-ttu-id="fdec6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdec6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdec6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdec6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fdec6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdec6-113">Not supported.</span></span>    |
|<span data-ttu-id="fdec6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdec6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdec6-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="fdec6-115">Device.Command</span></span>    |
|<span data-ttu-id="fdec6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdec6-116">Application</span></span> | <span data-ttu-id="fdec6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdec6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdec6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdec6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdec6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdec6-119">Request headers</span></span>

| <span data-ttu-id="fdec6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdec6-120">Header</span></span> |<span data-ttu-id="fdec6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fdec6-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="fdec6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdec6-122">Authorization</span></span>| <span data-ttu-id="fdec6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdec6-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fdec6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdec6-125">Accept</span></span> | <span data-ttu-id="fdec6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdec6-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="fdec6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdec6-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="fdec6-128">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="fdec6-128">List of actionStatus</span></span>

- <span data-ttu-id="fdec6-129">a solicitação,//comando foi criada e está aguardando processamento</span><span class="sxs-lookup"><span data-stu-id="fdec6-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="fdec6-130">o comando sentToTarget,//foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="fdec6-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="fdec6-131">executando,//dispositivo de destino confirmado o recebimento do comando e o está executando</span><span class="sxs-lookup"><span data-stu-id="fdec6-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="fdec6-132">conclusão da execução do comando//concluída</span><span class="sxs-lookup"><span data-stu-id="fdec6-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="fdec6-133">failedToSend,//Service falhou ao enviar comando para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="fdec6-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="fdec6-134">falha na execução do comando executionFailed,//</span><span class="sxs-lookup"><span data-stu-id="fdec6-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="fdec6-135">commandDropped,//comando Descartado pelo cliente se o dispositivo estiver no estado ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="fdec6-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="fdec6-136">cancelar,//cancelar o comando</span><span class="sxs-lookup"><span data-stu-id="fdec6-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="fdec6-137">Cancelando,//cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="fdec6-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="fdec6-138">o comando cancelado,//foi cancelado</span><span class="sxs-lookup"><span data-stu-id="fdec6-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="fdec6-139">repetir,//o serviço está tentando enviar novamente o comando para o destino</span><span class="sxs-lookup"><span data-stu-id="fdec6-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="fdec6-140">expirado,//o processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="fdec6-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="fdec6-141">erro,//erro interno ao processar o comando</span><span class="sxs-lookup"><span data-stu-id="fdec6-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="fdec6-142">status personalizado//personalizado</span><span class="sxs-lookup"><span data-stu-id="fdec6-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="fdec6-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdec6-143">Example</span></span>

<span data-ttu-id="fdec6-144">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdec6-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="fdec6-145">A ID do dispositivo é retornada ao emitir uma chamada GET para `/me/devices`, e a ID do comando é retornada ao realizar uma chamada post `/me/devices/{id}/command`em.</span><span class="sxs-lookup"><span data-stu-id="fdec6-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="fdec6-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdec6-146">Request</span></span>

<span data-ttu-id="fdec6-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdec6-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="fdec6-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdec6-148">Response</span></span>

<span data-ttu-id="fdec6-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fdec6-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="fdec6-150">Obter conteúdo do comando</span><span class="sxs-lookup"><span data-stu-id="fdec6-150">Get command payload</span></span>

<span data-ttu-id="fdec6-151">Obter uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdec6-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="fdec6-152">A carga de resposta é usada ao consultar um serviço de aplicativo para transportar dados de volta.</span><span class="sxs-lookup"><span data-stu-id="fdec6-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="fdec6-153">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdec6-153">Permissions</span></span>

<span data-ttu-id="fdec6-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdec6-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdec6-156">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdec6-156">Permission type</span></span>      | <span data-ttu-id="fdec6-157">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdec6-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdec6-158">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdec6-158">Delegated (work or school account)</span></span> | <span data-ttu-id="fdec6-159">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdec6-159">Not supported.</span></span>    |
|<span data-ttu-id="fdec6-160">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdec6-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdec6-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="fdec6-161">Device.Command</span></span>    |
|<span data-ttu-id="fdec6-162">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdec6-162">Application</span></span> | <span data-ttu-id="fdec6-163">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdec6-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="fdec6-164">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdec6-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="fdec6-165">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdec6-165">Request headers</span></span>

| <span data-ttu-id="fdec6-166">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdec6-166">Header</span></span> |<span data-ttu-id="fdec6-167">Valor</span><span class="sxs-lookup"><span data-stu-id="fdec6-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="fdec6-168">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdec6-168">Authorization</span></span>| <span data-ttu-id="fdec6-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdec6-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="fdec6-171">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdec6-171">Accept</span></span> | <span data-ttu-id="fdec6-172">application/json</span><span class="sxs-lookup"><span data-stu-id="fdec6-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="fdec6-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdec6-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="fdec6-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdec6-174">Example</span></span>

<span data-ttu-id="fdec6-175">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdec6-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="fdec6-176">A ID do dispositivo é retornada ao emitir uma chamada GET em `/me/devices`e a ID do comando é retornada ao executar uma chamada post em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="fdec6-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="fdec6-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdec6-177">Request</span></span>

<span data-ttu-id="fdec6-178">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdec6-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="fdec6-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdec6-179">Response</span></span>

<span data-ttu-id="fdec6-180">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fdec6-180">The following example shows the response.</span></span>

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
