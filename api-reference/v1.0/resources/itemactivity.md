---
author: daspek
title: tipo de recurso itemActivity
description: O objeto itemActivity fornece informações sobre uma atividade que ocorreu em um item.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2a22b78e517e3faf064073033ec1b4b9c582055d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089344"
---
# <a name="itemactivity-resource-type"></a>tipo de recurso itemActivity

Namespace: microsoft.graph

O **recurso itemActivity** fornece informações sobre atividades que ocorreram em um item ou em um contêiner.
Disponível atualmente só no SharePoint e no OneDrive for Business.

As ações que ocorreram dentro de um itemActivity são detalhadas na [propriedade itemActionSet.][]

>**Observação:** **itemActivity** está disponível apenas no SharePoint e OneDrive for Business.

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                    | Descrição
|:---------|:------------------------|:----------------------------------------
| id       | cadeia de caracteres                  | O identificador exclusivo da atividade. Somente leitura.
| access   | [accessAction][]        | Um item foi acessado.
| actor    | [identitySet][]         | Identidade de quem executou a ação. Somente leitura.
| activityDateTime    | DateTimeOffset | Detalhes sobre quando ocorreu a atividade. Somente leitura.

[accessAction]: accessaction.md
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
  "@type.aka&quot;: &quot;oneDrive.activityEntity"
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

