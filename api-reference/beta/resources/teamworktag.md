---
title: Tipo de recurso teamworkTag
description: Representa uma marca associada a uma equipe.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 677ddc348d1cd3ae152d7b777a6b29319839266c
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533896"
---
# <a name="teamworktag-resource-type"></a>Tipo de recurso teamworkTag

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma marca associada a uma equipe. 

As marcas fornecem uma maneira flexível para os clientes classificarem usuários ou grupos com base em um atributo comum dentro de uma equipe. Por exemplo, uma marca Desempresa, Gerente ou Designer permitirá que os usuários alcancem grupos de pessoas no Teams sem precisar digitar cada nome.

Quando uma marca é adicionada, os usuários podem @mention-la em um canal. Todos os que receberam essa marca receberão uma notificação da mesma forma que receberiam se fossem @mentioned individualmente. Os usuários também podem usar uma marca para iniciar um novo chat com os membros dessa marca.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar teamworkTags](../api/teamworktag-list.md)|[**coleção teamworkTag**](teamworktag.md)|Obter uma lista dos objetos **teamworkTag** e suas propriedades.|
|[Criar teamworkTag](../api/teamworktag-post.md)|[**teamworkTag**](teamworktag.md)|Crie um novo **objeto teamworkTag.**|
|[Obter teamworkTag](../api/teamworktag-get.md)|[**teamworkTag**](teamworktag.md)|Leia as propriedades e as relações de um **objeto teamworkTag.**|
|[Atualizar o teamworkTag](../api/teamworktag-update.md)|[**teamworkTag**](teamworktag.md)|Atualize as propriedades de um **objeto teamworkTag.**|
|[Excluir teamworkTag](../api/teamworktag-delete.md)|Nenhum|Excluir um **objeto teamworkTag.**|
|[Listar o trabalho em equipeTagMembers](../api/teamworktagmember-list.md)|[**coleção teamworkTagMember**](teamworktagmember.md)|Obter uma lista dos membros de uma marca padrão em uma equipe e suas propriedades.|
|[Criar trabalho em equipeTagMember](../api/teamworktagmember-post.md)|[**teamworkTagMember**](teamworktagmember.md)|Crie um novo **objeto teamworkTagMember.**|
|[Obter trabalho em equipeTagMember](../api/teamworktagmember-get.md)|[**teamworkTagMember**](teamworktagmember.md)|Obter as propriedades e as relações de um membro de uma marca padrão em uma equipe.|
|[Excluir o trabalho em equipeTagMember](../api/teamworktagmember-delete.md)|Nenhum|Exclua um membro de uma marca padrão na equipe.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição da marca como ela aparecerá para o usuário em Microsoft Teams.|
|displayName|String|Nome da marca como ele aparecerá para o usuário em Microsoft Teams.|
|id|String|ID da marca.|
|memberCount|Int32|O número de usuários atribuídos à marca.|
|tagType|teamworkTagType|O tipo de marca. O padrão é padrão.|
|teamId|Cadeia de Caracteres|ID da equipe na qual a marca é definida.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|membros|[coleção teamworkTagMember](../resources/teamworktagmember.md)|Usuários atribuídos à marca.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkTag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "String (identifier)",
  "teamId": "String",
  "displayName": "String",
  "memberCount": "Integer",
  "tagType": "String"
}
```

