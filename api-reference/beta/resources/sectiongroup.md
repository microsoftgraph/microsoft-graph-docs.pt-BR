---
title: tipo de recurso de @ @ @ Section
description: Um grupo de seções em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: dee2ca947af83f81f482ad280d0ae0c77b69fc56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087625"
---
# <a name="sectiongroup-resource-type"></a>tipo de recurso de @ @ @ Section

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de seções em um bloco de anotações do OneNote. Os grupos de seções podem conter seções e grupos de seções.

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
|createdDateTime|DateTimeOffset|A data e a hora em que o grupo de seções foi criado. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo do grupo de seções. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o grupo de seções foi modificado pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|displayName|Cadeia de caracteres|O nome do grupo de seção.|
|sectionGroupsUrl|Cadeia de caracteres|A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seção no grupo de seções. Somente leitura.|
|sectionsUrl|Cadeia de caracteres|A URL da `sections` propriedade de navegação, que retorna todas as seções no grupo de seções. Somente leitura.|
|própria|Cadeia de caracteres|O ponto de extremidade onde você pode obter detalhes sobre o grupo de seções. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|parentNotebook|[bloco de anotações](notebook.md)|O bloco de anotações que contém o grupo de seções. Somente leitura.|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|O grupo de seções que contém o grupo de seções. Somente leitura.|
|sectionGroups|coleção de [seções](sectiongroup.md)|Os grupos de seção na seção. Somente leitura. Anulável.|
|seções|coleção [onenoteSection](onenotesection.md)|As seções no grupo de seções. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter grupo de seções](../api/sectiongroup-get.md) | [sectionGroup](sectiongroup.md) |Leia as propriedades e as relações do grupo de seções.|
|[Criar grupo de seções](../api/sectiongroup-post-sectiongroups.md) |[sectionGroup](sectiongroup.md)| Crie um grupo de seção postando na coleção sectionGroups no grupo de seção especificado.|
|[List section groups](../api/sectiongroup-list-sectiongroups.md) |coleção de [seções](sectiongroup.md)| Obtém a coleção de grupos de seção no grupo de seção especificado.|
|[Criar seção](../api/sectiongroup-post-sections.md) |[onenoteSection](onenotesection.md)| Crie uma seção postando na coleção Sections no grupo de seção especificado.|
|[Listar seções](../api/sectiongroup-list-sections.md) |coleção [onenoteSection](onenotesection.md)| Obter uma coleção de seções no grupo de seção especificado.|

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


