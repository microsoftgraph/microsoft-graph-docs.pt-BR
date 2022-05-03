---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: non-product-specific
author: abheek-das
ms.openlocfilehash: 9a45cdff2bfdf1832400d6a563f2d7b1d64792de
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176612"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>Tipo de recurso multiValueLegacyExtendedProperty

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Uma propriedade estendida que contém uma coleção de valores.

Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | Uma instância de recurso com suporte: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md) ou [Outlook task](../resources/outlooktaskfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível. | Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível. |
|[Get](../api/multivaluelegacyextendedproperty-get.md) |Uma instância de recurso com [suporte (mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md)[, evento](../resources/event.md)[, calendário](../resources/calendar.md)[, contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa Outlook](../resources/outlooktask.md), [pasta de tarefas Outlook](../resources/outlooktaskfolder.md) ou postagem de [grupo)](../resources/post.md) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md). |Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|O identificador da propriedade. Somente leitura.|
|valor|coleção de cadeias de caracteres|Uma coleção de valores de propriedade.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


