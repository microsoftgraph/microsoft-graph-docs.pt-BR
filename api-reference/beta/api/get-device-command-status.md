---
title: Obter o status de comando do dispositivo
description: Obter o status de um comando em um dispositivo. Para obter a lista completa de códigos de status, confira lista de actionStatus.
localization_priority: Normal
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: 33470cb5aceb402d6a37749fa8c2ebcfcd0bce75
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807329"
---
# <a name="get-device-command-status"></a>Obter o status de comando do dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter o status de um comando em um dispositivo. Para obter a lista completa de códigos de status, confira [lista de actionStatus](#list-of-actionstatus).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Sem suporte.    |
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

- a solicitação,//comando foi criada e está aguardando processamento
- o comando sentToTarget,//foi enviado para o dispositivo de destino
- executando,//dispositivo de destino confirmado o recebimento do comando e o está executando
- conclusão da execução do comando//concluída
- failedToSend,//Service falhou ao enviar comando para o dispositivo de destino
- falha na execução do comando executionFailed,//
- commandDropped,//comando Descartado pelo cliente se o dispositivo estiver no estado ConnectedStandby
- cancelar,//cancelar o comando
- Cancelando,//cancelando o comando
- o comando cancelado,//foi cancelado
- repetir,//o serviço está tentando enviar novamente o comando para o destino
- expirado,//o processamento de comando excedeu o tempo de expiração
- erro,//erro interno ao processar o comando
- status personalizado//personalizado

## <a name="example"></a>Exemplo

Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo. A ID do dispositivo é retornada ao emitir uma chamada GET para `/me/devices` , e a ID do comando é retornada ao realizar uma chamada post em `/me/devices/{id}/command` .

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


## <a name="get-command-payload"></a>Obter conteúdo do comando

Obter uma carga de resposta para uma ação específica em um dispositivo. A carga de resposta é usada ao consultar um serviço de aplicativo para transportar dados de volta.


### <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Sem suporte.    |
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

Neste exemplo, você precisará da ID do dispositivo e da ID do comando que foi emitido para um dispositivo. A ID do dispositivo é retornada ao emitir uma chamada GET em `/me/devices` e a ID do comando é retornada ao executar uma chamada post em `/me/devices/{id}/command` .

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
