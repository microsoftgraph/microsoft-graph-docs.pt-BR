---
title: Comando Enviar dispositivo (preterido)
description: 'Essa API permite que os recursos do Project Rome comandom um dispositivo associado a uma conta da Microsoft. Depois de fazer uma chamada GET, `me/devices`passe a ID do dispositivo para emitir um comando para o dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os *parâmetros de tipo* *e conteúdo* . Para uma chamada do AppService, especifique o '
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: project-rome
author: ailae
ms.openlocfilehash: db99f797b234b96d83487765218d49c78d434c5f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944139"
---
# <a name="send-device-command-deprecated"></a>Comando Enviar dispositivo (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!CAUTION]
> Essa API foi preterida e parou de retornar dados em 30 de setembro de 2020.

Essa API permite que os recursos do Project Rome comandom um dispositivo associado a uma conta da Microsoft. Depois de fazer uma chamada GET, `me/devices`passe a ID do dispositivo para emitir um comando para o dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando LaunchURI, especifique os *parâmetros de tipo* *e conteúdo* . Para uma chamada appService, especifique os parâmetros *type*, *payload*, *packageFamilyName* e *appServiceName* .

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
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>Cabeçalhos de solicitação


| Cabeçalho |Valor
|:----|:------|
|Autorização| {token} de portador. Obrigatório. |
|Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON das propriedades do comando.

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
### <a name="command-properties"></a>Propriedades do comando

|**Nome**|**Tipo**|**Descrição**|
|:----|:------|:------|
|payload | microsoft.graph.json| Conteúdo a ser enviado para um serviço de aplicativo ou para iniciar um URI em um dispositivo. |
|responsePayload | microsoft.graph.json| Conteúdo retornado do dispositivo de destino. |
|postBackURI | Cadeia de caracteres | Poste o URI de volta para enviar notificações subsequentes de atualizações. |
|packageFamilyName | Cadeia de caracteres | Nome da Família de Pacotes do Windows do aplicativo. |
|appServiceName | Cadeia de caracteres | Nome do serviço de aplicativo definido pelo aplicativo de destino. Necessário se estiver iniciando um serviço de aplicativo. |
|type| Cadeia de caracteres | LaunchURI ou AppService. |
|id| String | A ID de um comando que foi enviado para o dispositivo. |
|actionStatus | Cadeia de caracteres | O [status](get-device-command-status.md) de um comando. |
|erro| Cadeia de caracteres| Todos os erros associados à solicitação do aplicativo de destino. |

## <a name="examples"></a>Exemplos

### <a name="example-1-launch-uri"></a>Exemplo 1: Iniciar URI

Veja a seguir um exemplo de uma solicitação LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino. Para iniciar um URI ou um aplicativo, emita um POST usando a ID do dispositivo (obtida da execução de uma chamada GET).`me/devices` Defina *os parâmetros* Type como *LaunchURI* e forneça um valor de URI como https://bing.com.

#### <a name="request"></a>Solicitação

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

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


### <a name="example-2-app-service"></a>Exemplo 2: Serviço de aplicativo

O exemplo a seguir mostra como consultar um serviço de aplicativo em um dispositivo. Para usar um serviço de aplicativo, você deve fazer uma chamada POST usando a ID do dispositivo (obtida da execução de uma chamada GET em `me/devices`). Para usar o exemplo a seguir, você deve instalar o aplicativo [Rome](https://aka.ms/romanapp) em seu dispositivo de destino.

Várias propriedades adicionais devem ser definidas na chamada.  O tipo deve ser definido como *AppService*, *AppServiceName* deve ser definido como o nome do serviço de aplicativo definido no aplicativo, *PackageFamilyName* deve ser definido como o nome da família de pacotes definido no manifesto do aplicativo e *o Payload* contém as chaves e os valores para o serviço que você está chamando dentro do aplicativo de destino.

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

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
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


