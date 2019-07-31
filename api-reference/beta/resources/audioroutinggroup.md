---
title: tipo de recurso audioRoutingGroup
description: O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: db5f94f9ac500dfeb97c6eb787783e9f749ae507
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974273"
---
# <a name="audioroutinggroup-resource-type"></a>tipo de recurso audioRoutingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.

> **Observação:** O [ConfigureMixer](../api/participant-configuremixer.md) não envolve nenhuma rota, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.

## <a name="methods"></a>Métodos

| Método                                                  | Tipo de retorno                               | Descrição                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Obter audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.|
| [Atualização](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Atualizar lista de receptores.                       |
| [Delete](../api/audioroutinggroup-delete.md)            | None                                      | Exclua o grupo roteamento de áudio.              |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | cadeia de caracteres            | Somente leitura. Servidor gerado.                                         |
| receptores     | collection(string) | Lista de IDs de participantes de recebimento.                                   |
| routingmode   | string            | Modo de grupo de roteamento.  Os valores possíveis são: `oneToOne` e `multicast`.   |
| fontes       | collection(string) | Lista de IDs de participantes de origem.                                      |

> **Observação:** O modo de roteamento determina as restrições nas fontes e nos receptores. Só há suporte para os seguintes grupos de roteamento.
> - `oneToOne`– fontes e receptores têm apenas um participante a cada.
> - `multicast`-a fonte tem um participante, mas há vários receptores. A lista de receptores pode ser atualizada.

> **Observação:** Se você criar muitos grupos de roteamento de áudio (por exemplo, um bot por participante), apenas o áudio dos quatro alto-falantes mais dominantes será encaminhado. Isso significa mesmo com o grupo de roteamento de áudio personalizado, se o alto-falante não estiver suficientemente alto no mixer principal, ele/ela não poderá ser ouvido pelo bot, mesmo se houver um grupo de áudio privado apenas para esse alto-falante e o bot.

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
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
