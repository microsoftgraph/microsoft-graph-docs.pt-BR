---
author: daspek
description: O recurso ItemActionSet fornece informações sobre as ações que com fizeram parte de um [activity][itemActivity] em um item.
ms.date: 09/14/2017
title: ItemActionSet
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d02467f8c4e780121ce8035b6aa09742a47c6f79
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724346"
---
# <a name="itemactionset-resource-type"></a>Tipo de recurso ItemActionSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **ItemActionSet** fornece informações sobre as ações que deram origem a uma [activity][itemActivity] em um item.

[itemActivity]: itemactivity.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka&quot;: &quot;oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a>Propriedades

Abaixo estão as ações disponíveis atualmente.
Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActionSet** sem quaisquer ações que seu aplicativo entenda.

| Propriedade | Tipo              | Descrição                       |
| :------- | :---------------- | :-------------------------------- |
| comment  | [commentAction][] | Um comentário foi adicionado ao item.  |
| create   | [createAction][]  | Um item foi criado.              |
| delete   | [deleteAction][]  | Um item foi excluído.              |
| edit     | [editAction][]    | Um item foi editado.               |
| mention  | [mentionAction][] | Um usuário foi mencionado no item. |
| move     | [moveAction][]    | Um item foi movido.                |
| rename   | [renameAction][]  | Um item foi renomeado.              |
| restore  | [restoreAction][] | Um item foi restaurado.             |
| share    | [shareAction][]   | Um item foi compartilhado.               |
| version  | [versionAction][] | Foi feito o controle de versão de um item.            |

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Comentários

Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
