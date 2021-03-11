---
title: Tipo de recurso sectionGroup
description: Um grupo de seção em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 6e52b922b9e882121ab926ca02f94089f9f55a0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719343"
---
# <a name="sectiongroup-resource-type"></a>Tipo de recurso sectionGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de seção em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sectionGroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora em que o grupo de seções foi criado. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo do grupo de seções. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o grupo de seções foi modificado pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do grupo de seção.|
|sectionGroupsUrl|Cadeia de caracteres|A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seções no grupo de seções. Somente leitura.|
|sectionsUrl|Cadeia de caracteres|A URL da `sections` propriedade de navegação, que retorna todas as seções no grupo de seções. Somente leitura.|
|self|Cadeia de caracteres|O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|parentNotebook|[bloco de anotações](notebook.md)|O bloco de anotações que contém o grupo de seções. Somente leitura.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|O grupo de seções que contém o grupo de seções. Somente leitura.|
|sectionGroups|[coleção sectionGroup](sectiongroup.md)|Os grupos de seção na seção. Somente leitura. Anulável.|
|seções|[Coleção onenoteSection](onenotesection.md)|As seções no grupo de seções. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter grupo de seções](../api/sectiongroup-get.md) | [sectionGroup](sectiongroup.md) |Leia as propriedades e as relações do grupo de seções.|
|[Criar grupo de seções](../api/sectiongroup-post-sectiongroups.md) |[sectionGroup](sectiongroup.md)| Crie um grupo de seções postando na coleção sectionGroups no grupo de seções especificado.|
|[List section groups](../api/sectiongroup-list-sectiongroups.md) |[coleção sectionGroup](sectiongroup.md)| Obter coleção de grupos de seções no grupo de seções especificado.|
|[Criar seção](../api/sectiongroup-post-sections.md) |[onenoteSection](onenotesection.md)| Crie uma seção postando na coleção sections no grupo de seções especificado.|
|[Listar seções](../api/sectiongroup-list-sections.md) |[Coleção onenoteSection](onenotesection.md)| Obter uma coleção de seções no grupo de seções especificado.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


