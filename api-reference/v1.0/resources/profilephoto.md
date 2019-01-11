---
title: Tipo de recurso de profilePhoto
description: Uma foto de perfil de um usuário, grupo ou contato do Outlook acessada do Exchange Online. Seus dados binários não são codificados em base 64.
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876563"
---
# <a name="profilephoto-resource-type"></a>Tipo de recurso de profilePhoto
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
|id|string|Somente leitura.|
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
