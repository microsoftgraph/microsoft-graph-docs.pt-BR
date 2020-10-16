---
title: 'aplicativo: setVerifiedPublisher'
description: Definir o distribuidor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9f56a4bf020003f71679c07f380c992b48db491
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471504"
---
# <a name="application-setverifiedpublisher"></a>aplicativo: setVerifiedPublisher

Namespace: microsoft.graph

Definir o [verifiedPublisher](../resources/verifiedPublisher.md) em um [aplicativo](../resources/application.md). Para obter mais informações, incluindo pré-requisitos para definir um editor verificado, confira [verificação do Publisher](/azure/active-directory/develop/publisher-verification-overview).

## <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte |
|Aplicativo | Sem suporte |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça as seguintes propriedades obrigatórias.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| verifiedPublisherId | cadeia de caracteres | O MPNID (Microsoft Partner Network ID) do editor verificado a ser definido no aplicativo, na conta do centro de parceiros do Publisher. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8c7a28dd-cebd-4dc0-b195-b2c7476e7a65
2020-09-09 21:28:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
