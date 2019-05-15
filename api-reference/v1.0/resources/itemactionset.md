---
author: daspek
ms.author: dspektor
title: Tipo de recurso ItemActionSet
description: O objeto doactionset fornece informações sobre as ações que foram realizadas como parte de uma atividade em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 065a6126e2e4a2f78cecfb2ae5497fac28e16899
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970599"
---
# <a name="itemactionset-resource-type"></a>tipo de recurso doactionset

O **** recurso doactionset fornece informações sobre as ações que compõem uma [atividade] [ itemActivity] em um item.

>**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.

[itemActivity]: itemactivity.md

## <a name="properties"></a>Propriedades

As ações a seguir estão disponíveis no momento. Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa **** lidar com um ItemAdded que inclui ações desconhecidas.

| Nome da propriedade | Tipo              | Descrição
|:--------------|:------------------|:-----------------------------------------
| comment       | [commentAction][] | Um comentário foi adicionado ao item.
| create        | [createAction][]  | Um item foi criado.
| delete        | [deleteAction][]  | Um item foi excluído.
| edit          | [editAction][]    | Um item foi editado.
| mention       | [mentionAction][] | Um usuário foi mencionado no item.
| move          | [moveAction][]    | Um item foi movido.
| rename        | [renameAction][]  | Um item foi renomeado.
| restore       | [restoreAction][] | Um item foi restaurado.
| share         | [shareAction][]   | Um item foi compartilhado.
| version       | [versionAction][] | Foi feito o controle de versão de um item.

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

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
