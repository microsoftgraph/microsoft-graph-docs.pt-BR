---
title: Obter o status de comando de dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa dos códigos de status, consulte a lista de actionStatus.
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510110"
---
# <a name="get-device-command-status"></a><span data-ttu-id="7cf64-104">Obter o status de comando de dispositivo</span><span class="sxs-lookup"><span data-stu-id="7cf64-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cf64-105">Obter o status de um comando em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cf64-105">Get the status of a command on a device.</span></span> <span data-ttu-id="7cf64-106">Para obter a lista completa dos códigos de status, consulte a [lista de actionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="7cf64-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cf64-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cf64-107">Permissions</span></span>

<span data-ttu-id="7cf64-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf64-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf64-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cf64-110">Permission type</span></span>      | <span data-ttu-id="7cf64-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cf64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf64-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cf64-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf64-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf64-113">Not supported.</span></span>    |
|<span data-ttu-id="7cf64-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cf64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf64-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="7cf64-115">Device.Command</span></span>    |
|<span data-ttu-id="7cf64-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cf64-116">Application</span></span> | <span data-ttu-id="7cf64-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf64-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cf64-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf64-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7cf64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf64-119">Request headers</span></span>

| <span data-ttu-id="7cf64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cf64-120">Header</span></span> |<span data-ttu-id="7cf64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7cf64-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="7cf64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cf64-122">Authorization</span></span>| <span data-ttu-id="7cf64-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cf64-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="7cf64-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cf64-125">Accept</span></span> | <span data-ttu-id="7cf64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cf64-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="7cf64-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf64-127">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="7cf64-128">Lista de actionStatus</span><span class="sxs-lookup"><span data-stu-id="7cf64-128">List of actionStatus</span></span>

- <span data-ttu-id="7cf64-129">solicitando, / / comando tiver sido criado e está aguardando processamento</span><span class="sxs-lookup"><span data-stu-id="7cf64-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="7cf64-130">sentToTarget, / / comando foi enviado para o dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="7cf64-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="7cf64-131">executá-lo, / / dispositivo alvo confirmados recebimento do comando e ele está em execução</span><span class="sxs-lookup"><span data-stu-id="7cf64-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="7cf64-132">concluída, / / execução concluída de comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="7cf64-133">failedToSend, / / Service falhou ao enviar um comando ao dispositivo de destino</span><span class="sxs-lookup"><span data-stu-id="7cf64-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="7cf64-134">executionFailed, / / falha na execução de comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="7cf64-135">commandDropped, / / comando ignoradas pelo cliente se o dispositivo está em estado ConnectedStandby</span><span class="sxs-lookup"><span data-stu-id="7cf64-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="7cf64-136">Cancelar, / / cancelar o comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="7cf64-137">Cancelando, / / cancelando o comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="7cf64-138">cancelado, / / comando foi cancelado</span><span class="sxs-lookup"><span data-stu-id="7cf64-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="7cf64-139">Repetir, / / serviço está repetindo para enviar o comando de destino</span><span class="sxs-lookup"><span data-stu-id="7cf64-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="7cf64-140">expirado, / / processamento de comando excedeu o tempo de expiração</span><span class="sxs-lookup"><span data-stu-id="7cf64-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="7cf64-141">erro, / / interno erro ao processar o comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="7cf64-142">personalizado / / personalizado status</span><span class="sxs-lookup"><span data-stu-id="7cf64-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="7cf64-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cf64-143">Example</span></span>

<span data-ttu-id="7cf64-144">Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cf64-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="7cf64-145">O dispositivo ID é retornada ao emitir um GET chamada `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="7cf64-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="7cf64-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf64-146">Request</span></span>

<span data-ttu-id="7cf64-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cf64-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="7cf64-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf64-148">Response</span></span>

<span data-ttu-id="7cf64-149">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cf64-149">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="7cf64-150">Obtenha a carga de comando</span><span class="sxs-lookup"><span data-stu-id="7cf64-150">Get command payload</span></span>

<span data-ttu-id="7cf64-151">Obtenha uma carga de resposta para uma ação específica em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cf64-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="7cf64-152">A carga de resposta é usada ao consultar um serviço de aplicativo para transportar os dados novamente.</span><span class="sxs-lookup"><span data-stu-id="7cf64-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="7cf64-153">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cf64-153">Permissions</span></span>

<span data-ttu-id="7cf64-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf64-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf64-156">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cf64-156">Permission type</span></span>      | <span data-ttu-id="7cf64-157">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cf64-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf64-158">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cf64-158">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf64-159">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf64-159">Not supported.</span></span>    |
|<span data-ttu-id="7cf64-160">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cf64-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf64-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="7cf64-161">Device.Command</span></span>    |
|<span data-ttu-id="7cf64-162">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cf64-162">Application</span></span> | <span data-ttu-id="7cf64-163">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf64-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="7cf64-164">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf64-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="7cf64-165">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf64-165">Request headers</span></span>

| <span data-ttu-id="7cf64-166">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cf64-166">Header</span></span> |<span data-ttu-id="7cf64-167">Valor</span><span class="sxs-lookup"><span data-stu-id="7cf64-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="7cf64-168">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cf64-168">Authorization</span></span>| <span data-ttu-id="7cf64-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cf64-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="7cf64-171">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cf64-171">Accept</span></span> | <span data-ttu-id="7cf64-172">application/json</span><span class="sxs-lookup"><span data-stu-id="7cf64-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="7cf64-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf64-173">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="7cf64-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cf64-174">Example</span></span>

<span data-ttu-id="7cf64-175">Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cf64-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="7cf64-176">O dispositivo ID é retornada ao emitir um GET chama em `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="7cf64-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="7cf64-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf64-177">Request</span></span>

<span data-ttu-id="7cf64-178">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cf64-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="7cf64-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf64-179">Response</span></span>

<span data-ttu-id="7cf64-180">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cf64-180">The following example shows the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
