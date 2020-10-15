---
title: 'aplicativo: setVerifiedPublisher'
description: Definir o fornecedor verificado de um aplicativo.
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cf02a44cbaff8494765bfa99383c3905f0522fe
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471544"
---
# <a name="application-setverifiedpublisher"></a>aplicativo: setVerifiedPublisher

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| verifiedPublisherId | string | O MPNID (Microsoft Partner Network ID) do editor verificado a ser definido no aplicativo, na conta do centro de parceiros do Publisher. |

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
POST https://graph.microsoft.com/beta/applications/{id}/setVerifiedPublisher
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

<!-- uuid: e7beba93-bb0b-42ea-96c8-231aa61d755e
2020-09-09 21:16:07 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
