---
title: Listar os dispositivos do usuário
description: Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto. Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para enviar um comando ao dispositivo.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bf6dff6b3eea14455bb9dc1e8eed2f515847efc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016937"
---
# <a name="list-user-devices"></a>Listar os dispositivos do usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista de dispositivos de usuário que dão suporte a recursos de Roma do projeto. Isso inclui a capacidade de iniciar um aplicativo ou uma mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada para mim/dispositivos, passe a ID do dispositivo para [enviar um comando](send-device-command.md) ao dispositivo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.    |
|Delegado (conta pessoal da Microsoft) | Device.Read    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho |Valor
|:----|:------|
|Autorização| {token} de portador. Obrigatório. |
|Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta 200 e as propriedades do dispositivo do usuário no corpo da resposta.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a>Exemplo
Este exemplo retornará a lista de dispositivos de um usuário. Para executar um comando em um dispositivo usando `me/devices/{id}/command` o, você precisará obter a ID do dispositivo que é retornado.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```


