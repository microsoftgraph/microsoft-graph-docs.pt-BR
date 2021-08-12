---
title: 'serviceUpdateMessage: favorite'
description: Altere o status de uma lista de mensagens de atualização de serviço para favoritos para o usuário inscrevado.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: bb1dba7788ba52dc925188a858f7d74c92b58f52590e05a7a991101c455fa118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54153529"
---
# <a name="serviceupdatemessage-favorite"></a>serviceUpdateMessage: favorite
Namespace: microsoft.graph

Altere o status de uma lista [de serviceUpdateMessages](../resources/serviceupdatemessage.md) como favorito para o usuário que está assinado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ServiceMessageViewpoint.Write|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/favorite
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|messageIds|String collection|Lista de IDs de mensagem para salvar como favorito.|

## <a name="response"></a>Resposta

Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um valor Boolean no corpo da `true` resposta. Caso contrário, `false` retornará no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_favorite"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/messages/favorite
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```
