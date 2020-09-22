---
author: JeremyKelley
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a2e1252437608d474e92346ed0aaba4a3a50053d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060024"
---
# <a name="shareddriveitem-resource-type"></a>Tipo de recurso SharedDriveItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **sharedDriveItem** é retornado ao se usar a API [Shares](../api/shares-get.md) para acessar um [driveItem](driveitem.md) compartilhado.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **sharedDriveItem**.

O recurso **sharedDriveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | Cadeia de caracteres                        | O identificador exclusivo do compartilhamento que está sendo acessado.              |
| name     | Cadeia de caracteres                        | O nome de exibição do item compartilhado.                             |
| owner    | [IdentitySet](identityset.md) | Informações sobre o proprietário do item compartilhado que está sendo referenciado. |

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                | Descrição
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem] | Usado para acessar o **driveItem** subjacente
| **list**          | [**list**][list]           | Usado para acessar a **lista** subjacente
| **listItem**      | [**listItem**][listItem]   | Usado para acessar o **listItem** subjacente
| **permissão**    | [**autorização**][permission] | Usado para acessar a **permissão** que representa o link de compartilhamento subjacente
| **site**          | [**site**][site]           | Usado para acessar o **site** subjacente

Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.

| Nome da relação | Tipo                         | Descrição
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | coleção [**driveItem**][driveItem] | Todos os driveItems contidos na raiz de compartilhamento. Não é possível enumerar esta coleção.
| **driveItem**     | [**driveItem**][driveItem]            | Usado para acessar o **driveItem** subjacente

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a>Métodos

| Método                                  | Caminho REST                |
| :-------------------------------------- | :----------------------- |
| [Obter item compartilhado](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->


