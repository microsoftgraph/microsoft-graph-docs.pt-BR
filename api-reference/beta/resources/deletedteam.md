---
title: Tipo de recurso deletedTeam
description: Representa uma equipe excluída no Microsoft Teams.
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de027a7e224db03f72fe424c1a4e08f5d238bea7
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578112"
---
# <a name="deletedteam-resource-type"></a>Tipo de recurso deletedTeam

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma [equipe](../resources/team.md) excluída no Microsoft Teams.

Cada equipe excluída está associada a um [grupo Microsoft 365](../resources/group.md). Para obter mais informações sobre como trabalhar com grupos e membros em equipes, consulte [Usar API do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[getAllMessages](../api/deletedteam-getallmessages.md)|[chatMessage](../resources/chatmessage.md) collection|Recuperar todas as [mensagens](../resources/chatmessage.md) entre todos os [canais](../resources/channel.md) em uma [equipe excluída](../resources/deletedteam.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID de uma equipe excluída. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|channels|Coleção [channel](../resources/channel.md)|Os canais que são compartilhados com esta equipe excluída ou criados nesta equipe excluída.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deletedTeam",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.deletedTeam",
    "id": "String (identifier)"
}
```

