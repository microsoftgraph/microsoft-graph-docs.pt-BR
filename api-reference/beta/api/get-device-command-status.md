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
# <a name="get-device-command-status"></a>Obter o status de comando do dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o status de um comando em um dispositivo. Para ver a lista completa de códigos de status, consulte [Lista de actionStatus](#list-of-actionstatus).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.    |
|Delegado (conta pessoal da Microsoft) | Device.Command    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho |Valor
|:----|:------|
|Autorização| {token} de portador. Obrigatório. |
|Aceitar | application/json |

## <a name="response"></a>Resposta
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

## <a name="list-of-actionstatus"></a>Lista de actionStatus

- solicitando, // O comando foi criado e está aguardando para ser processado
- sentToTarget, // Command foi enviado para o dispositivo de destino
- executing, // Target device acknowledged receipt of the command and is executing it
- concluída, // Execução de comando concluída
- failedToSend, // Service failed to send command to target device
- executionFailed, // Falha na execução do comando
- commandDropped, // Command dropped by client if device is in ConnectedStandby state
- cancel, // Cancel the command
- cancelando, // Cancelando o comando
- cancelado, // Command foi cancelado
- repetir, // O serviço está tentando novamente enviar o comando para o destino
- expirado, // Processamento de comando excedeu o tempo de expiração
- erro, // Erro interno durante o processamento do comando
- status personalizado // Personalizado

## <a name="example"></a>Exemplo

Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo. A ID do dispositivo é retornada ao emissão de uma chamada GET para , e a ID de comando é retornada ao fazer uma `/me/devices` chamada POST em `/me/devices/{id}/command` .

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.
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


## <a name="get-command-payload"></a>Obter carga de comando

Obter uma carga de resposta para uma ação específica em um dispositivo. A carga de resposta é usada ao consultar um serviço de aplicativo para carregar dados de volta.


### <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.    |
|Delegado (conta pessoal da Microsoft) | Device.Command    |
|Aplicativo | Sem suporte. |

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho |Valor
|:----|:------|
|Autorização| {token} de portador. Obrigatório. |
|Aceitar | application/json |

### <a name="response"></a>Resposta
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

### <a name="example"></a>Exemplo

Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo. A ID do dispositivo é retornada quando uma chamada GET é em emissão e a ID do comando é retornada ao fazer uma `/me/devices` chamada POST em `/me/devices/{id}/command` .

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

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


