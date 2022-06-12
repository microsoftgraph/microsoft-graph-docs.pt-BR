---
title: tipo de recurso section
description: Uma seção em um OneNote bloco de anotações. As seções podem conter páginas.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: 532bf71ff7963f4b70588d54d7d5f6b13c78332c
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034835"
---
# <a name="section-resource-type"></a>tipo de recurso section

Namespace: microsoft.graph

Uma seção em um OneNote bloco de anotações. As seções podem conter páginas.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora em que a seção foi criada. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da seção.  Somente leitura.|
|isDefault|Booliano|Indica se esta é a seção padrão do usuário. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a seção foi modificada pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|links|[SectionLinks](sectionlinks.md)|Links para abrir a seção. O `oneNoteClientURL` link abre a seção no OneNote cliente nativo se ele estiver instalado. O `oneNoteWebURL` link abre a seção no OneNote na Web.|
|displayName|Cadeia de caracteres|O nome da seção. |
|pagesUrl|Cadeia de caracteres|O `pages` ponto de extremidade em que você pode obter detalhes de todas as páginas na seção. Somente leitura.|
|Auto|Cadeia de caracteres|O ponto de extremidade em que você pode obter detalhes sobre a seção. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|páginas|Coleção [OnenotePage](page.md) |Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.|
|parentNotebook|[Notebook](notebook.md)|O bloco de anotações que contém a seção.  Somente leitura.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|O grupo de seções que contém a seção.  Somente leitura.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter seção](../api/section-get.md) | [OnenoteSection](section.md) |Leia as propriedades e as relações da seção.|
|[Create page](../api/section-post-pages.md) |[Page](page.md)| Crie uma página postando na coleção de páginas na seção especificada.|
|[List pages](../api/section-list-pages.md) |Coleção [Page](page.md)| Obtenha uma coleção de páginas na seção especificada.|
|[copyToNotebook](../api/section-copytonotebook.md)|Nenhum|Copie a seção para um bloco de anotações específico.|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|Nenhum|Copie a seção para um grupo de seções específico.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

