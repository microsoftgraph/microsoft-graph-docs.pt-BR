---
title: Obter o status de comando do dispositivo
description: Obter o status de um comando em um dispositivo. Para ver a lista completa de códigos de status, consulte Lista de actionStatus.
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: c0747438a9921f2ed6f3ccf1ee551f4aced70fcb
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515961"
---
# <a name="get-device-command-status"></a><span data-ttu-id="c099b-104">Obter o status de comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c099b-104">Get device command status</span></span>

<span data-ttu-id="c099b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c099b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c099b-106">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c099b-106">Get the status of a command on a device.</span></span> <span data-ttu-id="c099b-107">Para ver a lista completa de códigos de status, consulte [Lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="c099b-107">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="c099b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c099b-108">Permissions</span></span>

<span data-ttu-id="c099b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c099b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c099b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c099b-111">Permission type</span></span>      | <span data-ttu-id="c099b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c099b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c099b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c099b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c099b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c099b-114">Not supported.</span></span>    |
|<span data-ttu-id="c099b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c099b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c099b-116">Device.Command</span><span class="sxs-lookup"><span data-stu-id="c099b-116">Device.Command</span></span>    |
|<span data-ttu-id="c099b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c099b-117">Application</span></span> | <span data-ttu-id="c099b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c099b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c099b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c099b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c099b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c099b-120">Request headers</span></span>

| <span data-ttu-id="c099b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c099b-121">Header</span></span> |<span data-ttu-id="c099b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c099b-122">Value</span></span>
|:----|:------|
|<span data-ttu-id="c099b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c099b-123">Authorization</span></span>| <span data-ttu-id="c099b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c099b-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c099b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c099b-126">Accept</span></span> | <span data-ttu-id="c099b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c099b-127">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="c099b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c099b-128">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="c099b-129">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="c099b-129">List of actionStatus</span></span>

- <span data-ttu-id="c099b-130">solicitando, // O comando foi criado e está aguardando para ser processado</span><span class="sxs-lookup"><span data-stu-id="c099b-130">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="c099b-131">sentToTarget, // Command foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="c099b-131">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="c099b-132">executing, // Target device acknowledged receipt of the command and is executing it</span><span class="sxs-lookup"><span data-stu-id="c099b-132">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="c099b-133">concluída, // Execução de comando concluída</span><span class="sxs-lookup"><span data-stu-id="c099b-133">completed, // Command execution completed</span></span>
- <span data-ttu-id="c099b-134">failedToSend, // Service failed to send command to target device</span><span class="sxs-lookup"><span data-stu-id="c099b-134">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="c099b-135">executionFailed, // Falha na execução do comando</span><span class="sxs-lookup"><span data-stu-id="c099b-135">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="c099b-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span><span class="sxs-lookup"><span data-stu-id="c099b-136">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="c099b-137">cancel, // Cancel the command</span><span class="sxs-lookup"><span data-stu-id="c099b-137">cancel, // Cancel the command</span></span>
- <span data-ttu-id="c099b-138">cancelando, // Cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="c099b-138">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="c099b-139">cancelado, // Command foi cancelado</span><span class="sxs-lookup"><span data-stu-id="c099b-139">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="c099b-140">repetir, // O serviço está tentando novamente enviar o comando para o destino</span><span class="sxs-lookup"><span data-stu-id="c099b-140">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="c099b-141">expirado, // Processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="c099b-141">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="c099b-142">erro, // Erro interno durante o processamento do comando</span><span class="sxs-lookup"><span data-stu-id="c099b-142">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="c099b-143">status personalizado // Personalizado</span><span class="sxs-lookup"><span data-stu-id="c099b-143">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="c099b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c099b-144">Example</span></span>

<span data-ttu-id="c099b-145">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c099b-145">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="c099b-146">A ID do dispositivo é retornada ao emissão de uma chamada GET para , e a ID de comando é retornada ao fazer uma `/me/devices` chamada POST em `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="c099b-146">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="c099b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c099b-147">Request</span></span>

<span data-ttu-id="c099b-148">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c099b-148">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="c099b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c099b-149">Response</span></span>

<span data-ttu-id="c099b-150">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c099b-150">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="c099b-151">Obter carga de comando</span><span class="sxs-lookup"><span data-stu-id="c099b-151">Get command payload</span></span>

<span data-ttu-id="c099b-152">Obter uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c099b-152">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="c099b-153">A carga de resposta é usada ao consultar um serviço de aplicativo para carregar dados de volta.</span><span class="sxs-lookup"><span data-stu-id="c099b-153">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="c099b-154">Permissões</span><span class="sxs-lookup"><span data-stu-id="c099b-154">Permissions</span></span>

<span data-ttu-id="c099b-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c099b-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c099b-157">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c099b-157">Permission type</span></span>      | <span data-ttu-id="c099b-158">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c099b-158">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c099b-159">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c099b-159">Delegated (work or school account)</span></span> | <span data-ttu-id="c099b-160">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c099b-160">Not supported.</span></span>    |
|<span data-ttu-id="c099b-161">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c099b-161">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c099b-162">Device.Command</span><span class="sxs-lookup"><span data-stu-id="c099b-162">Device.Command</span></span>    |
|<span data-ttu-id="c099b-163">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c099b-163">Application</span></span> | <span data-ttu-id="c099b-164">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c099b-164">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="c099b-165">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c099b-165">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="c099b-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c099b-166">Request headers</span></span>

| <span data-ttu-id="c099b-167">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c099b-167">Header</span></span> |<span data-ttu-id="c099b-168">Valor</span><span class="sxs-lookup"><span data-stu-id="c099b-168">Value</span></span>
|:----|:------|
|<span data-ttu-id="c099b-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="c099b-169">Authorization</span></span>| <span data-ttu-id="c099b-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c099b-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="c099b-172">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c099b-172">Accept</span></span> | <span data-ttu-id="c099b-173">application/json</span><span class="sxs-lookup"><span data-stu-id="c099b-173">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="c099b-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="c099b-174">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="c099b-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c099b-175">Example</span></span>

<span data-ttu-id="c099b-176">Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c099b-176">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="c099b-177">A ID do dispositivo é retornada quando uma chamada GET é em emissão e a ID do comando é retornada ao fazer uma `/me/devices` chamada POST em `/me/devices/{id}/command` .</span><span class="sxs-lookup"><span data-stu-id="c099b-177">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="c099b-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c099b-178">Request</span></span>

<span data-ttu-id="c099b-179">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c099b-179">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="c099b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c099b-180">Response</span></span>

<span data-ttu-id="c099b-181">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="c099b-181">The following example shows the response.</span></span>

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


