---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
author: abheek-das
ms.openlocfilehash: 9f87c03e6a2d61fef478eed5554fc3a2d1e2de00
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736689"
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
|[Post](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | Uma instância de recurso com suporte: [mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md)[, evento](../resources/event.md)[,](../resources/contact.md) [calendário](../resources/calendar.md), contato, [contactFolder](../resources/contactfolder.md), tarefa do [Outlook](../resources/outlooktask.md) ou pasta de tarefas [do Outlook](../resources/outlooktaskfolder.md), mas não postagem em [grupo](../resources/post.md). | Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível. |
|[Get](../api/singlevaluelegacyextendedproperty-get.md) |Uma ou uma coleção de instâncias de recursos com [suporte (mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md)[, evento](../resources/event.md)[, calendário](../resources/calendar.md)[, contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), tarefa do [Outlook](../resources/outlooktask.md), pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md) ou postagem de [grupo) ou](../resources/post.md) uma dessas instâncias expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md). |Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.|

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


