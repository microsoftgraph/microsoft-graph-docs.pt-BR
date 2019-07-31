---
title: tipo de recurso outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 631da782e47325a2ff28eb6ae9eb1447e1b0a14d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009255"
---
# <a name="outlooktaskfolder-resource-type"></a>tipo de recurso outlookTaskFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ). 

No Outlook, o grupo de tarefas padrão `My Tasks`, contém uma pasta de tarefas padrão `Tasks`,, para a caixa de correio do usuário. Não é possível renomear ou excluir essas pastas e o grupo de tarefas padrão, mas você pode criar grupos de tarefas e pastas de tarefas adicionais.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Obtenha as propriedades e os relacionamentos da pasta de tarefas especificada do Outlook.|
|[Criar outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Criar uma tarefa do Outlook na pasta de tarefas especificada.|
|[Listar tarefas](../api/outlooktaskfolder-list-tasks.md) |coleção [outlookTask](outlooktask.md)| Obter todas as tarefas do Outlook na pasta especificada.|
|[Atualização](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook. |
|[Delete](../api/outlooktaskfolder-delete.md) | Nenhum |Excluir a pasta de tarefas do Outlook especificada.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Crie uma ou mais propriedades estendidas de valor único em uma pasta de tarefas Nova ou existente do Outlook.   |
|[Obter pasta de tarefas com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Obter pastas de tarefas do Outlook que contenham uma propriedade estendida `$expand` de `$filter`valor único usando ou. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma pasta de tarefas Nova ou existente do Outlook.  |
|[Obter pasta de tarefas com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade estendida de `$expand`vários valores usando. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|String|A versão da pasta de tarefas.|
|id|String|O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário. Somente leitura.|
|isDefaultFolder|Booliano|True se a pasta é a pasta de tarefas padrão.|
|name|String|O nome da pasta de tarefas.|
|parentGroupKey|Guid|O identificador exclusivo do GUID para o grupo pai da pasta de tarefas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de vários valores definida para a pasta de tarefas. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de valor único definidas para a pasta de tarefas. Somente leitura. Anulável.|
|tarefas|coleção [outlookTask](outlooktask.md)|As tarefas nesta pasta de tarefas. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}-->

```json
{
  "changeKey": "String",
  "id": "String (identifier)",
  "isDefaultFolder": true,
  "name": "String",
  "parentGroupKey": "Guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
