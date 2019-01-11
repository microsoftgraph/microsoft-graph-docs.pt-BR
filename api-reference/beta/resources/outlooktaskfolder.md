---
title: tipo de recurso de outlookTaskFolder
description: 'Uma pasta que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4b4c4bade46022b30c6e4e1f50aae58d32656f0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882926"
---
# <a name="outlooktaskfolder-resource-type"></a>tipo de recurso de outlookTaskFolder

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma pasta que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ). 

No Outlook, o grupo de tarefas padrão, `My Tasks`, contém uma pasta de tarefas padrão, `Tasks`, para caixa de correio do usuário. Não é possível renomear ou excluir esses grupo de tarefa padrão e uma pasta, mas você pode criar grupos de tarefas adicionais e pastas de tarefa.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTaskFolder](../api/outlooktaskfolder-get.md) | [outlookTaskFolder](outlooktaskfolder.md) |Obtenha as propriedades e relacionamentos da pasta de tarefas do Outlook especificado.|
|[Criar outlookTask](../api/outlooktaskfolder-post-tasks.md) |[outlookTask](outlooktask.md)| Crie uma tarefa do Outlook na pasta tarefa especificada.|
|[Listar tarefas](../api/outlooktaskfolder-list-tasks.md) |coleção [outlookTask](outlooktask.md)| Obtenha todas as tarefas do Outlook na pasta especificada.|
|[Update](../api/outlooktaskfolder-update.md) | [outlookTaskFolder](outlooktaskfolder.md)   |Atualize as propriedades graváveis de uma pasta de tarefas do Outlook. |
|[Delete](../api/outlooktaskfolder-delete.md) | Nenhum |Exclua a pasta de tarefas do Outlook especificada.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[outlookTaskFolder](outlooktaskfolder.md)  |Crie um ou mais propriedades estendidas de valor único em uma pasta de tarefas do Outlook nova ou existente.   |
|[Obter a pasta de tarefas com a propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Obtenha as pastas de tarefas do Outlook que contêm um valor único propriedade estendida usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [outlookTaskFolder](outlooktaskfolder.md) | Crie um ou mais propriedades estendidas de valores múltiplos em uma pasta de tarefas do Outlook nova ou existente.  |
|[Obter a pasta de tarefas com vários valores de propriedade estendida](../api/multivaluelegacyextendedproperty-get.md)  | [outlookTaskFolder](outlooktaskfolder.md) | Obtenha uma pasta de tarefas do Outlook que contenha uma propriedade de valor múltiplos estendida usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|Cadeia de caracteres|A versão da pasta de tarefas.|
|id|Cadeia de caracteres|O identificador da pasta de tarefas, exclusivo na caixa de correio do usuário. Somente leitura.|
|isDefaultFolder|Booliano|True se a pasta está na pasta de tarefas padrão.|
|name|Cadeia de caracteres|O nome da pasta de tarefas.|
|parentGroupKey|Guid|O identificador GUID exclusivo para o grupo do pai da pasta tarefa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de múltiplos valores definidos para a pasta de tarefas. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)|A coleção de propriedades estendidas de valor único definidos para a pasta de tarefas. Somente leitura. Anulável.|
|tarefas|coleção [outlookTask](outlooktask.md)|As tarefas nesta pasta tarefa. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "multiValueExtendedProperties",
    "singleValueExtendedProperties",
    "tasks"
  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
