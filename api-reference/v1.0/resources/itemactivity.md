---
author: daspek
ms.author: dspektor
title: tipo de recurso de multiatividade
description: O objeto myactivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536684"
---
# <a name="itemactivity-resource-type"></a>tipo de recurso de multiatividade

O **** recurso doactivity fornece informações sobre as atividades que ocorreram em um item ou em um contêiner.
Disponível atualmente só no SharePoint e no OneDrive for Business.

As ações que ocorreram em um ItemProperty são detalhadas na propriedade itempropertyset. [][]

>**Observação:** **** o myactivity atualmente só está disponível no SharePoint e no onedrive for Business.

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                    | Descrição
|:---------|:------------------------|:----------------------------------------
| id       | string                  | O identificador exclusivo da atividade. Somente leitura.
| Access   | [accessaction][]        | Um item foi acessado.
| actor    | [identitySet][]         | Identidade de quem executou a ação. Somente leitura.
| activityDateTime    | DateTimeOffset | Detalhes sobre quando ocorreu a atividade. Somente leitura.

[accessaction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a>Relações

| Nome da relação | Tipo          | Descrição
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | Expõe o **driveItem** ao qual essa atividade direcionou.
| listItem          | [listItem][]  | Expõe o **listItem** ao qual essa atividade direcionou.

[driveItem]: driveitem.md
[listItem]: listitem.md

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
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
