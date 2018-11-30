---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
ms.openlocfilehash: 7c8cdab7adc705333d1aeaad526aeeb813de10a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039497"
---
# <a name="itemactivity-resource-type"></a>Tipo de recurso ItemActivity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **ItemActivity** fornece informações sobre atividades que ocorreram em um item ou dentro de um repositório.
Disponível atualmente só no SharePoint e no OneDrive for Business.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                    | Descrição
|:---------|:------------------------|:----------------------------------------
| id       | string                  | O identificador exclusivo da atividade. Somente leitura.
| acesso   | [accessAction][]        | Um item foi acessado.
| action   | [itemActionSet][]       | Detalhes sobre a ação que ocorreu. Somente leitura.
| actor    | [identitySet][]         | Identidade de quem executou a ação. Somente leitura.
| location | [location][]            | Local físico onde a ação foi realizada. Somente leitura.
| times    | [itemActivityTimeSet][] | Detalhes sobre quando ocorreu a atividade. Somente leitura.

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>Relações

| Nome da relação | Tipo          | Descrição
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | Expõe o **driveItem** ao qual essa atividade direcionou.
| listItem          | [listItem][]  | Expõe o **listItem** ao qual essa atividade direcionou.

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>Ações

As ações que ocorreram dentro de uma atividade são detalhadas na propriedade **action**.
Abaixo estão as ações disponíveis atualmente.
Novas ações podem ser registradas no futuro, portanto, verifique se o seu aplicativo tem tolerância à manipulação de um **itemActivity** sem quaisquer ações que seu aplicativo entenda.

| Nome da ação | Tipo              | Descrição
|:------------|:------------------|:-------------------------------------------
| comment     | [commentAction][] | Um comentário foi adicionado ao item.
| create      | [createAction][]  | Um item foi criado.
| delete      | [deleteAction][]  | Um item foi excluído.
| edit        | [editAction][]    | Um item foi editado.
| mention     | [mentionAction][] | Um usuário foi mencionado no item.
| move        | [moveAction][]    | Um item foi movido.
| rename      | [renameAction][]  | Um item foi renomeado.
| restore     | [restoreAction][] | Um item foi restaurado.
| share       | [shareAction][]   | Um item foi compartilhado.
| version     | [versionAction][] | Foi feito o controle de versão de um item.

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>Comentários

**ItemActivity** está disponível atualmente só no SharePoint e no OneDrive for Business.

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity"
} -->
