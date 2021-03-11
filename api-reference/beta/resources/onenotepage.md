---
title: Tipo de recurso do onenotePage
description: Uma página em um bloco de anotações do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 2f8a93080b3eaa58be95e8721307cdde31b359ea
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719448"
---
# <a name="onenotepage-resource-type"></a>Tipo de recurso do onenotePage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma página em um bloco de anotações do OneNote.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|conteúdo|Fluxo|Conteúdo HTML da página.|
|contentUrl|Cadeia de caracteres|A URL do conteúdo HTML da página.  Somente leitura.|
|createdByAppId|Cadeia de caracteres|O identificador exclusivo do aplicativo que criou a página. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora em que a página foi criada. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da página.  Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a página foi modificada pela última vez. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|level|Int32|O nível de recuo da página. Somente leitura.|
|links|[pageLinks](pagelinks.md)|Links para abrir a página. O `oneNoteClientURL` link abre a página no cliente nativo do OneNote se estiver instalado. O `oneNoteWebUrl` link abre a página no OneNote na Web. Somente leitura.|
|order|Int32|A ordem da página em sua seção pai. Somente leitura.|
|self|Cadeia de caracteres|O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.|
|title|Cadeia de caracteres|O título da página. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|parentNotebook|[bloco de anotações](notebook.md)|O bloco de anotações que contém a página.  Somente leitura.|
|parentSection|[onenoteSection](onenotesection.md)|A seção que contém a página. Somente leitura.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter página](../api/page-get.md) | [onenotePage](onenotepage.md) |Leia as propriedades e as relações da página.|
|[Atualizar conteúdo da página](../api/page-update.md) | Nenhum(a) |Atualize o conteúdo HTML da página. |
|[Excluir página](../api/page-delete.md) | Nenhum(a) |Exclua a página. |
|[copyToSection](../api/page-copytosection.md)| Nenhum(a) |Copia a página para uma seção específica.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


