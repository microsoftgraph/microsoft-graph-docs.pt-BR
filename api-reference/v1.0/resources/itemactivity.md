---
author: daspek
ms.author: dspektor
title: tipo de recurso de multiatividade
description: O objeto myactivity fornece informações sobre uma atividade que ocorreu em um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4ae71056fccebcb372891124b01999004b1957c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009328"
---
# <a name="itemactivity-resource-type"></a>tipo de recurso de multiatividade

Namespace: microsoft.graph

O recurso **doactivity** fornece informações sobre as atividades que ocorreram em um item ou em um contêiner.
Disponível atualmente só no SharePoint e no OneDrive for Business.

As ações que ocorreram em um ItemProperty são detalhadas [na propriedade][] itempropertyset.

>**Observação:** o **myactivity** atualmente só está disponível no SharePoint e no onedrive for Business.

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

