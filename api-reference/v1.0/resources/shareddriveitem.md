---
author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: O recurso sharedDriveItem é retornado ao se usar a API Shares para acessar um driveItem compartilhado.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da14e18c21f122646c7b7b86f3bc9e5401a60d8882762c4e4e096beecfda2cd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251747"
---
# <a name="shareddriveitem-resource-type"></a>Tipo de recurso SharedDriveItem

Namespace: microsoft.graph

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
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | Cadeia de caracteres                        | O identificador exclusivo do compartilhamento que está sendo acessado.              |
| nome     | Cadeia de caracteres                        | O nome de exibição do item compartilhado.                             |
| owner    | [IdentitySet](identityset.md) | Informações sobre o proprietário do item compartilhado que está sendo referenciado. |

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                | Descrição
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Usado para acessar o **driveItem** subjacente
| **list**          | [**list**][list]        | Usado para acessar a **lista** subjacente
| **listItem**      | [**listItem**][listItem]    | Usado para acessar o **listItem** subjacente
| **permissão**    | [**permission**][permission] | Usado para acessar a **permissão** que representa o link de compartilhamento subjacente
| **site**          | [**site**][site]        | Usado para acessar o **site** subjacente

Como alternativa, para **driveItems** compartilhados de contas pessoais do OneDrive, as relações a seguir também podem ser usadas.

| Nome da relação | Tipo                         | Descrição
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**Coleção driveItem**][driveItem] | Todos os driveItems contidos na raiz de compartilhamento. Não é possível enumerar este conjunto.
| **root**          | [**driveItem**][driveItem]   | Usado para acessar o **driveItem** subjacente. Preterido - use em `driveItem` vez disso.

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

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

