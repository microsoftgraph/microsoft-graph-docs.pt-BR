---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7d1293b42108b785848b2e351186020e06d46ca4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037231"
---
# <a name="profilephoto-resource-type"></a>Tipo de recurso de profilePhoto

Namespace: microsoft.graph

Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.

Os tamanhos de fotos em HD compatíveis com o Exchange Online são os seguintes: “48x48”, “64x64”, “96x96”, “120x120”, “240x240”, “360x360”, “432x432”, “504x504” e “648x648”.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get profilePhoto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) |Obtenha a **profilePhoto** especificada ou seus metadados (propriedades de profilePhoto).|
|[Update](../api/profilephoto-update.md) | [profilePhoto](profilephoto.md)  |Atribua uma foto para o usuário, grupo ou contato especificado. A foto deve estar em formato binário. Ela substitui a foto existente, se houver.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|cadeia de caracteres|Somente leitura.|
|height|int32|A altura da foto. Somente leitura.|
|width|int32|A largura da foto. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

