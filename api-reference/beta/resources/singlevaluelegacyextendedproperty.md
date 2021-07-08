---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 578b2792a815dd0c7cd5dad4fc77d9c96319045a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334581"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a>Tipo de recurso singleValueLegacyExtendedProperty

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Uma propriedade estendida que contém um único valor.

Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | Uma instância de recurso suportada: [mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md) [,](../resources/event.md)evento [,](../resources/contact.md) [calendário](../resources/calendar.md), contato , [contactFolder,](../resources/contactfolder.md) [Outlook tarefa](../resources/outlooktask.md)ou Outlook [pasta](../resources/outlooktaskfolder.md)de tarefas , mas não postagem de [grupo](../resources/post.md). | Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível. |
|[Get](../api/singlevaluelegacyextendedproperty-get.md) |Uma ou uma coleção de instância de recurso com suporte[(](../resources/message.md)mensagem , [mailFolder](../resources/mailfolder.md) [,](../resources/event.md)evento [,](../resources/contact.md) [calendário](../resources/calendar.md), contato , [contactFolder](../resources/contactfolder.md), [Outlook](../resources/outlooktask.md)tarefa, pasta de tarefa [Outlook](../resources/outlooktaskfolder.md)ou postagem de grupo [)](../resources/post.md)ou uma instância expandida com um [único objetoValueLegacyExtendedProperty.](singlevaluelegacyextendedproperty.md) |Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|string|O identificador da propriedade. Somente leitura.|
|valor|string|Um valor de propriedade.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


