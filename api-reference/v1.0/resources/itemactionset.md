---
author: daspek
title: Tipo de recurso ItemActionSet
description: O objeto itemActionSet fornece informações sobre as ações que ocorreram como parte de uma atividade em um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 665ffbe2a34eeeb40735ba539c10eae00b5f0e0d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089358"
---
# <a name="itemactionset-resource-type"></a>Tipo de recurso itemActionSet

Namespace: microsoft.graph

O **recurso itemActionSet** fornece informações sobre as ações que com fizeram parte de uma [atividade][itemActivity] em um item.

>**Observação:** No momento, os registros de atividade do item estão disponíveis apenas SharePoint e OneDrive for Business.

[itemActivity]: itemactivity.md

## <a name="properties"></a>Propriedades

As ações a seguir estão disponíveis no momento. Como novas ações podem ser adicionadas no futuro, certifique-se de que seu aplicativo possa manipular **um itemActionSet** que inclui ações desconhecidas.

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

