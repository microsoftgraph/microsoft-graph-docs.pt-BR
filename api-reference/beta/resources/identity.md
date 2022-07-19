---
author: JeremyKelley
title: tipo de recurso de identidade
description: Representa uma identidade de um ator.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 80c48a178bcc2e82848d245df3383e792eec01f3
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855872"
---
# <a name="identity-resource-type"></a>tipo de recurso de identidade

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade de um _ator_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.

Em algumas circunstâncias, o identificador exclusivo do ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   | Descrição                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | String | O nome de exibição da identidade. Observe que isso pode nem sempre estar disponível ou atualizado. Por exemplo, se um usuário alterar o nome de exibição, a API poderá mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecerão como tendo sido alterados ao usar [delta](../api/driveitem-delta.md).  |
| id                  | Cadeia de caracteres | Identificador exclusivo da identidade.                                                                                                                                                                                                                                                                                   |
| tenantId            | String | Identidade exclusiva do locatário (opcional).                                                                                                                                                                                                                                                                             |

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


