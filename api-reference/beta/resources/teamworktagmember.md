---
title: Tipo de recurso teamworkTagMember
description: Representa um usuário em uma equipe que tem uma marca aplicada a ele.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 73666dd19720e6d8882bb16fd90c612097e41d10
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059870"
---
# <a name="teamworktagmember-resource-type"></a>Tipo de recurso teamworkTagMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em uma equipe à qual uma marca é aplicada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar o trabalho em equipeTagMembers](../api/teamworktagmember-list.md)|**coleção teamworkTagMember**|Obter uma lista dos membros de uma marca padrão em uma equipe e suas propriedades.|
|[Obter trabalho em equipeTagMember](../api/teamworktagmember-get.md)|**teamworkTagMember**|Obter as propriedades e as relações de um membro de uma marca padrão em uma equipe.|
|[Excluir o trabalho em equipeTagMember](../api/teamworktagmember-delete.md)|Nenhum|Exclua um membro de uma marca padrão na equipe.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do membro.|
|ID|String|ID do membro.|
|tenantID|String|A ID do locatário do que o membro da marca faz parte.|
|userID|String|A ID do usuário do membro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "ID",
  "@odata.type": "microsoft.graph.teamworkTagMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagMember",
  "ID": "String (Identifier)",
  "displayName": "String",
  "tenantID": "String",
  "userID": "String"
}
```

