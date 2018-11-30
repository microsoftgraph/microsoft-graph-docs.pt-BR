---
title: Obter o status de comando de dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa dos códigos de status, consulte a lista de actionStatus.
ms.openlocfilehash: 1e51d3b4366e87d9802518a50fe348d3ba0f250d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033019"
---
# <a name="get-device-command-status"></a><span data-ttu-id="92123-104">Obter o status de comando de dispositivo</span><span class="sxs-lookup"><span data-stu-id="92123-104">Get device command status</span></span>

> <span data-ttu-id="92123-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92123-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92123-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92123-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92123-107">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92123-107">Get the status of a command on a device.</span></span> <span data-ttu-id="92123-108">Para obter a lista completa dos códigos de status, consulte a [lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="92123-108">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="92123-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="92123-109">Permissions</span></span>

<span data-ttu-id="92123-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92123-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92123-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92123-112">Permission type</span></span>      | <span data-ttu-id="92123-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92123-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92123-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92123-114">Delegated (work or school account)</span></span> | <span data-ttu-id="92123-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92123-115">Not supported.</span></span>    |
|<span data-ttu-id="92123-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92123-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92123-117">Device.Command</span><span class="sxs-lookup"><span data-stu-id="92123-117">Device.Command</span></span>    |
|<span data-ttu-id="92123-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92123-118">Application</span></span> | <span data-ttu-id="92123-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92123-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92123-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92123-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92123-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92123-121">Request headers</span></span>

| <span data-ttu-id="92123-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92123-122">Header</span></span> |<span data-ttu-id="92123-123">Valor</span><span class="sxs-lookup"><span data-stu-id="92123-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="92123-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92123-124">Authorization</span></span>| <span data-ttu-id="92123-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92123-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="92123-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92123-127">Accept</span></span> | <span data-ttu-id="92123-128">application/json</span><span class="sxs-lookup"><span data-stu-id="92123-128">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="92123-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92123-129">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="92123-130">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="92123-130">List of actionStatus</span></span>

- <span data-ttu-id="92123-131">solicitando, / / comando tiver sido criado e está aguardando processamento</span><span class="sxs-lookup"><span data-stu-id="92123-131">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="92123-132">sentToTarget, / / comando foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="92123-132">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="92123-133">executá-lo, / / dispositivo alvo confirmados recebimento do comando e ele está em execução</span><span class="sxs-lookup"><span data-stu-id="92123-133">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="92123-134">concluída, / / execução concluída de comando</span><span class="sxs-lookup"><span data-stu-id="92123-134">completed, // Command execution completed</span></span>
- <span data-ttu-id="92123-135">failedToSend, / / Service falhou ao enviar um comando ao dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="92123-135">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="92123-136">executionFailed, / / falha na execução de comando</span><span class="sxs-lookup"><span data-stu-id="92123-136">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="92123-137">commandDropped, / / comando ignoradas pelo cliente se o dispositivo está em estado ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="92123-137">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="92123-138">Cancelar, / / cancelar o comando</span><span class="sxs-lookup"><span data-stu-id="92123-138">cancel, // Cancel the command</span></span>
- <span data-ttu-id="92123-139">Cancelando, / / cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="92123-139">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="92123-140">cancelado, / / comando foi cancelado</span><span class="sxs-lookup"><span data-stu-id="92123-140">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="92123-141">Repetir, / / serviço está repetindo para enviar o comando de destino</span><span class="sxs-lookup"><span data-stu-id="92123-141">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="92123-142">expirado, / / processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="92123-142">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="92123-143">erro, / / interno erro ao processar o comando</span><span class="sxs-lookup"><span data-stu-id="92123-143">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="92123-144">personalizado / / personalizado status</span><span class="sxs-lookup"><span data-stu-id="92123-144">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="92123-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92123-145">Example</span></span>

<span data-ttu-id="92123-146">Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92123-146">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="92123-147">O dispositivo ID é retornada ao emitir um GET chamada `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="92123-147">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="92123-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92123-148">Request</span></span>

<span data-ttu-id="92123-149">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="92123-149">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="92123-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="92123-150">Response</span></span>

<span data-ttu-id="92123-151">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="92123-151">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="get-command-payload"></a><span data-ttu-id="92123-152">Obtenha a carga de comando</span><span class="sxs-lookup"><span data-stu-id="92123-152">Get command payload</span></span>

<span data-ttu-id="92123-153">Obtenha uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92123-153">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="92123-154">A carga de resposta é usada ao consultar um serviço de aplicativo para transportar os dados novamente.</span><span class="sxs-lookup"><span data-stu-id="92123-154">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="92123-155">Permissions</span><span class="sxs-lookup"><span data-stu-id="92123-155">Permissions</span></span>

<span data-ttu-id="92123-p108">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92123-p108">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92123-158">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92123-158">Permission type</span></span>      | <span data-ttu-id="92123-159">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92123-159">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92123-160">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92123-160">Delegated (work or school account)</span></span> | <span data-ttu-id="92123-161">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92123-161">Not supported.</span></span>    |
|<span data-ttu-id="92123-162">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92123-162">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92123-163">Device.Command</span><span class="sxs-lookup"><span data-stu-id="92123-163">Device.Command</span></span>    |
|<span data-ttu-id="92123-164">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92123-164">Application</span></span> | <span data-ttu-id="92123-165">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92123-165">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="92123-166">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92123-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="92123-167">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92123-167">Request headers</span></span>

| <span data-ttu-id="92123-168">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92123-168">Header</span></span> |<span data-ttu-id="92123-169">Valor</span><span class="sxs-lookup"><span data-stu-id="92123-169">Value</span></span>
|:----|:------|
|<span data-ttu-id="92123-170">Autorização</span><span class="sxs-lookup"><span data-stu-id="92123-170">Authorization</span></span>| <span data-ttu-id="92123-p109">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92123-p109">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="92123-173">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92123-173">Accept</span></span> | <span data-ttu-id="92123-174">application/json</span><span class="sxs-lookup"><span data-stu-id="92123-174">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="92123-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="92123-175">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="92123-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92123-176">Example</span></span>

<span data-ttu-id="92123-177">Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92123-177">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="92123-178">O dispositivo ID é retornada ao emitir um GET chama em `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="92123-178">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="92123-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92123-179">Request</span></span>

<span data-ttu-id="92123-180">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="92123-180">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="92123-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="92123-181">Response</span></span>

<span data-ttu-id="92123-182">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="92123-182">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
