---
title: Atualizar o grupo de roteamento de áudio
description: Modificar fontes e receptores de um audioRoutingGroup.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b12d93d3cd8255cb735beaba7c78684a2b3b3a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833835"
---
# <a name="update-audio-routing-group"></a>Atualizar o grupo de roteamento de áudio

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Modificar fontes e receptores de um [audioRoutingGroup](../resources/audioroutinggroup.md).

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                |
| :-------------- | :--------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Não suportado                       |
| Delegado (conta pessoal da Microsoft) | Não suportado                       |
| Aplicativo     | Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
| receptores | String collection | Os participantes de destino no audioRoutingGroup. |
| routingMode | String | Os valores possíveis são: `oneToOne` e `multicast`. |
| sources | String collection | O participante de origem no audioRoutingGroup. |

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [audioRoutingGroup](../resources/audioroutinggroup.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```
##### <a name="response"></a>Resposta

> **Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
