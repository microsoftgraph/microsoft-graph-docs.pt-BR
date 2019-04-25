---
title: Enviar comando do dispositivo
description: 'Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft. Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* . Para uma chamada serviço, especifique o '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537522"
---
# <a name="send-device-command"></a>Enviar comando do dispositivo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft. Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* . Para uma chamada serviço, especifique os parâmetros *Type*, *Payload*, *packageFamilyName*e *appServiceName* .

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
## <a name="command-properties"></a>Propriedades de comando 

|**Nome**|**Tipo**|**Descrição**|
|:----|:------|:------|
|payload | Microsoft. Graph. JSON| Carga a ser enviada a um serviço de aplicativo ou para iniciar um URI em um dispositivo. |
|responsePayload | Microsoft. Graph. JSON| Carga retornada do dispositivo de destino. |
|postBackURI | String | Postar URI para enviar notificações de atualizações subsequentes. |
|packageFamilyName | String | Nome do aplicativo da família de pacote do Windows. |
|appServiceName | String | Nome do serviço de aplicativo definido pelo aplicativo de destino. Necessário se iniciar um serviço de aplicativo. |
|type| String | LaunchURI ou serviço. |
|id| Cadeia de caracteres | A ID de um comando que foi enviado ao dispositivo. |
|actionStatus | String | O [status](get-device-command-status.md) de um comando. |
|erro| String| Quaisquer erros associados à solicitação do aplicativo de destino. |

## <a name="launch-uri-example"></a>Exemplo de URI de inicialização

Aqui está um exemplo de uma solicitação LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino. Para iniciar um URI ou um aplicativo, emita uma POSTAgem usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`). Defina os parâmetros de *tipo* como *LaunchURI* e forneça um valor de URI https://bing.comcomo.

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


## <a name="app-service-example"></a>Exemplo de serviço de aplicativo

Veja um exemplo de consulta de um serviço de aplicativo em um dispositivo. Para usar um serviço de aplicativo, você deve fazer uma chamada POST usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`). Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.

Várias propriedades adicionais devem ser definidas na chamada. O *tipo* deve ser definido *como serviço*, *AppServiceName* deve ser definido como o nome do serviço de aplicativo definido no aplicativo, *PackageFamilyName* deve ser definido como o nome da família do pacote definido no manifesto do aplicativo e *carga* contém as chaves e os valores para o serviço que você está chamando no aplicativo de destino.

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
