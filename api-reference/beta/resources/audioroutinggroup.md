---
title: tipo de recurso audioRoutingGroup
description: O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543998"
---
# <a name="audioroutinggroup-resource-type"></a>tipo de recurso audioRoutingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O grupo de roteamento de áudio armazena uma rota de áudio privada entre os participantes de uma conversa de várias partes. Source é o próprio participante e os receptores são um subconjunto de outros participantes da conversa de vários participantes.

> **Observação:** O [ConfigureMixer](../api/participant-configuremixer.md) não envolve nenhuma rota, é para toda a chamada para definir os níveis de volume para combinações de receptor de origem.

## <a name="methods"></a>Métodos

| Método                                                  | Tipo de retorno                               | Descrição                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Obter audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Leia as propriedades e os relacionamentos do objeto audioRoutingGroup.|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Atualizar lista de receptores.                       |
| [Excluir](../api/audioroutinggroup-delete.md)            | None                                      | Exclua o grupo roteamento de áudio.              |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo              | Descrição                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | Somente leitura. Servidor gerado.                                         |
| receptores     | String Collection | Lista de IDs de participantes de recebimento.                                   |
| routingmode   | String            | Modo de grupo de roteamento.  Os valores possíveis são: `oneToOne` e `multicast`.   |
| fontes       | String Collection | Lista de IDs de participantes de origem.                                      |

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
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
