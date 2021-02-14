---
author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 717426f29b8c466af5799871fcc12cf4cd8bdf65
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239090"
---
# <a name="baseitem-resource-type"></a>Tipo de recurso BaseItem

Namespace: microsoft.graph

O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:

* [drive](drive.md)
* [driveItem](driveitem.md)
* [site](site.md)
* [sharedDriveItem](shareddriveitem.md)

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **baseItem**.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo              | Descrição                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| id                   | string            | O identificador exclusivo da unidade. Somente leitura.                                         |
| createdBy            | [identitySet][]   | Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.        |
| createdDateTime      | dateTimeOffset    | Data e hora de criação do item. Somente leitura.                                             |
| description          | Cadeia de caracteres            | Fornece uma descrição do item visível para o usuário. Opcional.                             |
| eTag                 | string            | ETag do item. Somente leitura.                                                          |
| lastModifiedBy       | [identitySet][]   | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura. |
| lastModifiedDateTime | dateTimeOffset    | Data e hora em que o item foi modificado pela última vez. Somente leitura.                                   |
| nome                 | string            | O nome do item. Leitura e gravação.                                                      |
| parentReference      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.                              |
| webUrl               | string (url)      | URL que exibe o recurso no navegador. Somente leitura.                              |

## <a name="relationships"></a>Relações

| Relação       | Tipo     | Descrição
|:-------------------|:---------|:---------------------------------------------
| createdByUser      | [user][] | A identidade do usuário que criou o item. Somente leitura.
| lastModifiedByUser | [user][] | A identidade do usuário que modificou o item pela última vez. Somente leitura.

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a>Comentários

O tipo `baseItem` não deve ser usado diretamente.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

