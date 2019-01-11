---
title: Tipo de recurso sectionGroup
description: Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.
localization_priority: Normal
ms.openlocfilehash: 9e955d91fa49642100694da66421665a0d67b3da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855423"
---
# <a name="sectiongroup-resource-type"></a>Tipo de recurso sectionGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um grupo de seção em um bloco de anotações do OneNote. Grupos de seção podem conter seções e grupos de seção.

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
  "@odata.type": "microsoft.graph.sectiongroup"
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
|createdDateTime|DateTimeOffset|A data e hora da criação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String|O identificador exclusivo do grupo de seção. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do grupo de seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|displayName|String|O nome do grupo de seção.|
|sectionGroupsUrl|String|A URL da propriedade de navegação `sectionGroups`, que retorna todos os grupos de seção no grupo de seção. Somente leitura.|
|sectionsUrl|String|A URL da propriedade de navegação `sections`, que retorna todas as seções no grupo de seção. Somente leitura.|
|self|String|O ponto de extremidade onde você pode obter detalhes sobre o grupo de seção. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|O bloco de anotações que contém o grupo de seção. Somente leitura.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|O grupo de seção que contém o grupo de seção. Somente leitura.|
|sectionGroups|Coleção [SectionGroup](sectiongroup.md)|Os grupos de seção na seção. Somente leitura. Anulável.|
|sections|Coleção [Section](section.md)|As seções no grupo de seção. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get section group](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |Leia as propriedades e as relações do grupo de seção.|
|[Criar grupo de seção](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Crie um grupo de seção postando na coleção sectionGroups do grupo de seção especificado.|
|[Listar grupos de seção](../api/sectiongroup-list-sectiongroups.md) |Coleção [SectionGroup](sectiongroup.md)| A coleção de grupos de seção no grupo de seção especificado.|
|[Criar seção](../api/sectiongroup-post-sections.md) |[Section](section.md)| Crie uma seção postando na coleção sections do grupo de seção especificado.|
|[Listar seções](../api/sectiongroup-list-sections.md) |Coleção [Section](section.md)| Obtenha uma coleção de seções no grupo de seção especificado.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
