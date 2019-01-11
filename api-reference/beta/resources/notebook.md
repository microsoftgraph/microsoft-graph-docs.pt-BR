---
title: Tipo de recurso notebook
description: Um bloco de anotações do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: c39ac85dcfacb332a72c81d1d5f075a7a5021047
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876556"
---
# <a name="notebook-resource-type"></a>Tipo de recurso notebook

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um bloco de anotações do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e hora da criação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String|O identificador exclusivo do bloco de anotações. Somente leitura.|
|isDefault|Booliano|Indica se este é o bloco de anotações padrão do usuário. Somente leitura.|
|isShared|Booliano|Indica se o bloco de anotações é compartilhado. Se for verdadeiro, o conteúdo do bloco de anotações poderá ser visto por pessoas que não sejam o proprietário. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|links|[NotebookLinks](notebooklinks.md)|Links para abrir o bloco de anotações. O link `oneNoteClientURL` abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre o bloco de anotações no OneNote Online.|
|displayName|String|O nome do bloco de anotações.|
|sectionGroupsUrl|String|A URL da propriedade de navegação `sectionGroups` que retorna todos os grupos de seção no bloco de anotações. Somente leitura.|
|sectionsUrl|String|A URL da propriedade de navegação `sections` que retorna todas as seções no bloco de anotações. Somente leitura.|
|self|String|O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações. Somente leitura.|
|userRole|String|Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`. O proprietário representa o acesso no nível de proprietário ao bloco de anotações. O proprietário representa o acesso de leitura/gravação ao bloco de anotações. O leitor representa o acesso somente leitura ao bloco de anotações. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|sectionGroups|Coleção [SectionGroup](sectiongroup.md)|Obtém os grupos de seção no bloco de anotações. Somente leitura. Anulável.|
|sections|Coleção [Section](section.md)|As seções no bloco de anotações. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter bloco de anotações](../api/notebook-get.md) | [Notebook](notebook.md) |Leia as propriedades e as relações do bloco de anotações.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | coleção [recentNotebook](recentnotebook.md) | Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário. |
|[Criar grupo de seção](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Crie um grupo de seção postando na coleção sectionGroups no bloco de anotações especificado.|
|[Listar grupos de seção](../api/notebook-list-sectiongroups.md) |Coleção [SectionGroup](sectiongroup.md)| Obtenha uma coleção de grupos de seção no bloco de anotações especificado.|
|[Criar seção](../api/notebook-post-sections.md) |[Section](section.md)| Crie uma seção postando na coleção sections no bloco de anotações especificado.|
|[Listar seções](../api/notebook-list-sections.md) |Coleção [Section](section.md)| Obtenha uma coleção de seções no bloco de anotações especificado.|
|[copyNotebook](../api/notebook-copynotebook.md)| None | Copia um bloco de anotações.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
