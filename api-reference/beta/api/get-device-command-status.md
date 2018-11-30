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
# <a name="get-device-command-status"></a>Obter o status de comando de dispositivo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Obter o status de um comando em um dispositivo. Para obter a lista completa dos códigos de status, consulte a [lista de actionStatus](#list-of-actionstatus).

## <a name="permissions"></a>Permissions

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

- solicitando, / / comando tiver sido criado e está aguardando processamento
- sentToTarget, / / comando foi enviado para o dispositivo de destino
- executá-lo, / / dispositivo alvo confirmados recebimento do comando e ele está em execução
- concluída, / / execução concluída de comando
- failedToSend, / / Service falhou ao enviar um comando ao dispositivo de destino
- executionFailed, / / falha na execução de comando
- commandDropped, / / comando ignoradas pelo cliente se o dispositivo está em estado ConnectedStandby
- Cancelar, / / cancelar o comando
- Cancelando, / / cancelando o comando
- cancelado, / / comando foi cancelado
- Repetir, / / serviço está repetindo para enviar o comando de destino
- expirado, / / processamento de comando excedeu o tempo de expiração
- erro, / / interno erro ao processar o comando
- personalizado / / personalizado status

## <a name="example"></a>Exemplo

Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo. O dispositivo ID é retornada ao emitir um GET chamada `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.

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


## <a name="get-command-payload"></a>Obtenha a carga de comando

Obtenha uma carga de resposta para uma ação específica em um dispositivo. A carga de resposta é usada ao consultar um serviço de aplicativo para transportar os dados novamente.


### <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.    |
|Delegado (conta pessoal da Microsoft) | Device.Command    |
|Aplicativo | Sem suporte. |

### <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
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

Neste exemplo, será necessário o ID do dispositivo e a ID do comando que tenha sido emitido para um dispositivo. O dispositivo ID é retornada ao emitir um GET chama em `/me/devices`, e o comando ID é retornada ao realizar uma POSTAGEM chama em `/me/devices/{id}/command`.

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
