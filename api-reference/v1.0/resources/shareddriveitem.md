---
author: JeremyKelley
title: Tipo de recurso sharedDriveItem
ms.localizationpriority: medium
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 52fa1c8d4395283f6e33464142eab0f411fd46ac
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034583"
---
# <a name="shareddriveitem-resource-type"></a>Tipo de recurso sharedDriveItem

Namespace: microsoft.graph

O **recurso sharedDriveItem** é retornado ao usar a API [de](../api/shares-get.md) compartilhamentos para acessar um [driveItem compartilhado](driveitem.md).

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
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | Cadeia de caracteres                        | O identificador exclusivo do compartilhamento que está sendo acessado.              |
| nome     | Cadeia de caracteres                        | O nome de exibição do item compartilhado.                             |
| owner    | [identitySet](identityset.md) | Informações sobre o proprietário do item compartilhado que está sendo referenciado. |

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                | Descrição
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Usado para acessar o **driveItem** subjacente
| **list**          | [**list**][list]        | Usado para acessar a **lista** subjacente
| **listItem**      | [**listItem**][listItem]    | Usado para acessar o **listItem** subjacente
| **permissão**    | [**Permissão**][permission] | Usado para acessar a permissão **que** representa o link de compartilhamento subjacente
| **site**          | [**site**][site]        | Usado para acessar o **site** subjacente

Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.

| Nome da relação | Tipo                         | Descrição
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**coleção driveItem**][driveItem] | Todos os driveItems contidos na raiz de compartilhamento. Não é possível enumerar este conjunto.
| **root**          | [**driveItem**][driveItem]   | Usado para acessar o **driveItem subjacente**. Preterido – use em `driveItem` vez disso.

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

Para obter mais informações sobre as facetas em um DriveItem, consulte [driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

