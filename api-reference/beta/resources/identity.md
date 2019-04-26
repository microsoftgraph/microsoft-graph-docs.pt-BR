---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
ms.openlocfilehash: a2ba76d5bac372be0a40001028dfb54e690a14fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333664"
---
# <a name="identity-resource-type"></a>tipo de recurso Identity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   | Descrição                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | String | Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).  |
| id                  | Cadeia de caracteres | Identificador exclusivo da identidade.                                                                                                                                                                                                                                                                                   |
| tenantId            | String | Identidade exclusiva do locatário (opcional).                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a>Comentários

Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->
