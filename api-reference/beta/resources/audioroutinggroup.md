---
title: tipo de recurso audioRoutingGroup
description: O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb96e83f6c80a3b3c50b37612731272ca329e3cc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913748"
---
# <a name="audioroutinggroup-resource-type"></a>tipo de recurso audioRoutingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.

> **Observação:** o [ConfigureMixer](../api/participant-configuremixer.md) não envolve nenhuma rota, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.

## <a name="methods"></a>Methods

| Método                                                  | Tipo de retorno                               | Descrição                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Obter audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Atualizar lista de receptores.                       |
| [Delete](../api/audioroutinggroup-delete.md)            | None                                      | Exclua o grupo roteamento de áudio.              |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | cadeia de caracteres            | Somente leitura.                                                           |
| receptores     | collection(string) | Lista de IDs de participantes de recebimento.                                   |
| routingmode   | cadeia de caracteres            | Modo de grupo de roteamento.  Os valores possíveis são: `oneToOne` e `multicast`.   |
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
