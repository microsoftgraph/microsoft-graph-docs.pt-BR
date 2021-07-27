---
title: Tipo de recurso teamworkTagMember
description: Representa um usuário em uma equipe que tem uma marca aplicada a ele.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: b8e6d70a8249168383f2bc1b0e6d8884525855ec
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534513"
---
# <a name="teamworktagmember-resource-type"></a>Tipo de recurso teamworkTagMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um usuário em uma equipe à qual uma marca é aplicada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar o trabalho em equipeTagMembers](../api/teamworktagmember-list.md)|[**coleção teamworkTagMember**](teamworktagmember.md)|Obter uma lista dos membros de uma marca padrão em uma equipe e suas propriedades.|
|[Criar trabalho em equipeTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|Crie um novo **objeto teamworkTagMember.**|
|[Obter trabalho em equipeTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|Obter as propriedades e as relações de um membro de uma marca padrão em uma equipe.|
|[Excluir o trabalho em equipeTagMember](../api/teamworktagmember-delete.md)|Nenhum|Exclua um membro de uma marca padrão na equipe.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do membro.|
|ID|Cadeia de Caracteres|ID do membro.|
|tenantID|Cadeia de Caracteres|A ID do locatário do que o membro da marca faz parte.|
|userID|Cadeia de Caracteres|A ID do usuário do membro.|

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

