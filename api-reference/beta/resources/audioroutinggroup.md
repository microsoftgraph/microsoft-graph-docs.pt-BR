---
title: tipo de recurso de audioRoutingGroup
description: O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes. Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e18a9beb660b9bae0c1bbe1034ec64790d369fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980185"
---
# <a name="audioroutinggroup-resource-type"></a>tipo de recurso de audioRoutingGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O grupo de roteamento áudio armazena uma rota de áudio privada entre os participantes em uma conversa com vários participantes. Fonte é o participante propriamente dito e os receptores são um subconjunto dos outros participantes da conversa com vários participantes.

> **Observação:** [ConfigureMixer](../api/participant-configuremixer.md) não envolvem quaisquer rotas, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.

## <a name="methods"></a>Métodos

| Método                                                  | Tipo de retorno                               | Descrição                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Obter audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Lista de receptores de atualização.                       |
| [Delete](../api/audioroutinggroup-delete.md)            | Nenhum                                      | Exclua o grupo de roteamento de áudio.              |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | Somente leitura. Servidor foi gerado.                                         |
| receptores     | Coleção de cadeia de caracteres | Lista de recebimento de ids de participante.                                   |
| routingMode   | String            | Modo de grupo de roteamento.  Os valores possíveis são: `oneToOne` e `multicast`.   |
| sources       | Coleção de cadeia de caracteres | Lista de ids de participante de origem.                                      |

> **Observação:** Modo de roteamento determina as restrições nas fontes e receptores. Há suporte para os seguintes grupos de roteamento.
> - `oneToOne`-fontes e receptores possuem apenas um participante.
> - `multicast`-fonte com um participante, mas há vários receptores. Lista de receptores pode ser atualizada.

> **Observação:** Se você criar vários grupos de roteamento áudio (por exemplo, um bot de cada participante), somente o áudio de superior 4 dominantes alto-falantes será encaminhado. Isso significa que mesmo com o grupo de roteamento personalizados áudio, se o alto-falante não está alto o suficiente no Misturador de principal, ele/ela não possa ser ouvido pelo bot, mesmo se não houver um grupo de áudio privado apenas para este alto-falante e o bot.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
