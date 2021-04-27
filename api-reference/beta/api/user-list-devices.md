---
title: Listar os dispositivos do usuário
description: Obter uma lista de dispositivos de usuário que suportam Project de Roma. Isso inclui a capacidade de iniciar um aplicativo ou mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada GET em mim/dispositivos, passe a ID do dispositivo para enviar um comando para seu dispositivo.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b116213a285cc334d02a70ed94461b5cf6436eea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036293"
---
# <a name="list-user-devices"></a>Listar os dispositivos do usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de dispositivos de usuário que suportam Project de Roma. Isso inclui a capacidade de iniciar um aplicativo ou mensagem ou enviar dados para um aplicativo. Depois de fazer uma chamada GET em mim/dispositivos, passe a ID do dispositivo para [enviar um comando](send-device-command.md) para seu dispositivo.

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
Este exemplo retornará a lista de dispositivos para um usuário. Para comando de um dispositivo usando `me/devices/{id}/command` , você precisará obter a ID do dispositivo retornado.

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

Este é um exemplo de resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

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


