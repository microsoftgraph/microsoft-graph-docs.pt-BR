---
title: Enviar um comando de dispositivo
description: 'Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando. Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Dois tipos de comandos são suportados: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* . Para uma chamada de AppService, especifique o '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891984"
---
# <a name="send-device-command"></a>Enviar um comando de dispositivo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Essa API permite que os recursos de projeto Roma para um dispositivo associado a uma conta da Microsoft de comando. Depois de fazer uma chamada GET em `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Dois tipos de comandos são suportados: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os parâmetros de *tipo* e da *carga* . Para uma chamada de AppService, especifique o *tipo*, *carga*, *packageFamilyName*e *appServiceName* parâmetros.

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
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>Cabeçalhos de solicitação


| Cabeçalho |Valor
|:----|:------|
|Autorização| {token} de portador. Obrigatório. |
|Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON das propriedades do comando.

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>Resposta

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a>Propriedades de comando 

|**Name**|**Tipo**|**Descrição**|
|:----|:------|:------|
|payload | Microsoft.Graph.JSON| Carga para enviar para um serviço do aplicativo ou iniciar um URI em um dispositivo. |
|responsePayload | Microsoft.Graph.JSON| Carga retornado do dispositivo de destino. |
|postBackURI | Cadeia de caracteres | URI para enviar notificações subsequentes das atualizações de volta de postagem. |
|packageFamilyName | Cadeia de caracteres | Nome da família Windows pacote de aplicativo. |
|appServiceName | Cadeia de caracteres | Nome do serviço de aplicativo definido pelo aplicativo de destino. Será necessário se lançar um serviço do aplicativo. |
|type| Cadeia de caracteres | LaunchURI ou AppService. |
|id| Cadeia de caracteres | A identificação de um comando que foi enviado ao dispositivo. |
|actionStatus | Cadeia de caracteres | O [status](get-device-command-status.md) de um comando. |
|erro| Cadeia de caracteres| Quaisquer erros associados à solicitação do aplicativo de destino. |

## <a name="launch-uri-example"></a>Exemplo URI de início

Aqui está um exemplo de uma solicitação de LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino. Para iniciar um aplicativo ou um URI, emitir um POST usando a ID do dispositivo (obtido fazendo uma chamada GET em `me/devices`). Definir os parâmetros de *tipo* para *LaunchURI* e fornecer um valor URI, tais como https://bing.com.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a>Resposta 

Este é um exemplo de resposta.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a>Exemplo de aplicativo do serviço

Aqui está um exemplo de uma consulta de um serviço de aplicativo em um dispositivo. Para usar um serviço de aplicativo, você deve fazer uma chamada de POSTAGEM usando a id do dispositivo (obtido fazendo uma chamada GET em `me/devices`). Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.

Várias outras propriedades devem ser definidas na chamada. *Tipo* deve ser definida como *AppService*, *AppServiceName* deve ser definida com o nome da definida no aplicativo de serviço do aplicativo, *PackageFamilyName* deve ser definida como o nome da família de pacote definido no manifesto do aplicativo e *carga* contém as chaves e valores para o serviço que você está chamando dentro do aplicativo de destino.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
