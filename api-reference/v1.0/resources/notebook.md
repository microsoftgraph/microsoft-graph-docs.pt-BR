---
title: tipo de recurso Notebook
description: Um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2259a8d84c3c784c5c6af5ffda08a863a818be1a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086505"
---
# <a name="notebook-resource-type"></a>tipo de recurso Notebook

Namespace: microsoft.graph

Um bloco de anotações do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
|createdDateTime|DateTimeOffset|A data e a hora em que o bloco de anotações foi criado. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo do bloco de anotações. Somente leitura.|
|isDefault|Booliano|Indica se este é o bloco de anotações padrão do usuário. Somente leitura.|
|isShared|Booliano|Indica se o bloco de anotações é compartilhado. Se for true, o conteúdo do bloco de anotações poderá ser visto por pessoas que não o proprietário. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|links|[NotebookLinks](notebooklinks.md)|Links para abrir o bloco de anotações. O `oneNoteClientURL` link abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado. O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.|
|displayName|Cadeia de caracteres|O nome do bloco de anotações.|
|sectionGroupsUrl|Cadeia de caracteres|A URL da `sectionGroups` propriedade de navegação, que retorna todos os grupos de seção no bloco de anotações. Somente leitura.|
|sectionsUrl|Cadeia de caracteres|A URL da `sections` propriedade de navegação, que retorna todas as seções do bloco de anotações. Somente leitura.|
|própria|Cadeia de caracteres|O ponto de extremidade onde você pode obter detalhes sobre o bloco de anotações. Somente leitura.|
|userRole|onenoteUserRole|Os valores possíveis são: `Owner`, `Contributor`, `Reader`, `None`. O proprietário representa o acesso no nível do proprietário ao bloco de anotações. O colaborador representa acesso de leitura/gravação ao bloco de anotações. O leitor representa acesso somente leitura ao bloco de anotações. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|sectionGroups|Coleção [SectionGroup](sectiongroup.md)|Obtém os grupos de seção no bloco de anotações. Somente leitura. Anulável.|
|seções|Coleção [OnenoteSection](section.md)|As seções no bloco de anotações. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter bloco de anotações](../api/notebook-get.md) | [Notebook](notebook.md) |Leia as propriedades e as relações do bloco de anotações.|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | coleção [recentNotebook](recentnotebook.md) | Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário. |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [Notebook](notebook.md) | Recupere as propriedades e os relacionamentos de um objeto Notebook usando seu caminho de URL. |
|[Criar grupo de seções](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| Criar um grupo de seção postando na coleção sectionGroups no bloco de anotações especificado.|
|[List section groups](../api/notebook-list-sectiongroups.md) |Coleção [SectionGroup](sectiongroup.md)| Obtém uma coleção de grupos de seções no bloco de anotações especificado.|
|[Criar seção](../api/notebook-post-sections.md) |[OnenoteSection](section.md)| Criar uma seção postando na coleção Sections no bloco de anotações especificado.|
|[Listar seções](../api/notebook-list-sections.md) |Coleção [OnenoteSection](section.md)| Obtém uma coleção de seções no bloco de anotações especificado.|
|[copyNotebook](../api/notebook-copynotebook.md)| Nenhum | Copia um bloco de anotações.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

