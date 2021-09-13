---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48e333f4109170281dce075d6106075f3afa666d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032304"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a>Tipo de recurso multiValueLegacyExtendedProperty

Namespace: microsoft.graph

Uma propriedade estendida que contém uma coleção de valores.

Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Post](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível. | Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível. |
|[Get](../api/multivaluelegacyextendedproperty-get.md) |Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md). |Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|O identificador da propriedade. Somente leitura.|
|valor|coleção de cadeias de caracteres|Uma coleção de valores de propriedade.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

