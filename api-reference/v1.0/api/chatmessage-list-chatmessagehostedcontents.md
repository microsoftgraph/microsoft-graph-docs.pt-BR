---
title: Listar chatMessageHostedContents
description: Recupere a lista de objetos chatMessageHostedContent de uma mensagem.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16dc59427eeab168d816780c9fcdc5c6603a1955
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634284"
---
# <a name="list-hostedcontents"></a>Listar hostedContents

Namespace: microsoft.graph

Recupere a lista de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) de uma mensagem.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Para **recurso de** canal: ChannelMessage.Read.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Para **recurso** de canal: ChannelMessage.Read.Group*, ChannelMessage.Read.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).

> [!NOTE]
> É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {código}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos chatMessageHostedContent](../resources/chatmessagehostedcontent.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> [!NOTE]
> O objeto de resposta mostrado aqui pode ser reduzido para a capacidade de leitura. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


