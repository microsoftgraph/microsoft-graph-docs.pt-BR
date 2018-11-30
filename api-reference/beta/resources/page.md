---
title: Tipo de recurso page
description: Uma página em um bloco de anotações do OneNote.
ms.openlocfilehash: 82b9ca00cb4488c33e73daa94844b11f8de301cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038650"
---
# <a name="page-resource-type"></a>Tipo de recurso page

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma página em um bloco de anotações do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
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
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|content|Fluxo|O conteúdo HTML da página.|
|contentUrl|String|A URL do conteúdo HTML da página.  Somente leitura.|
|createdByAppId|String|O identificador exclusivo do aplicativo que criou a página. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String|O identificador exclusivo da página.  Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última modificação da página. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|nível|Int32|O nível de recuo da página. Somente leitura.|
|links|[PageLinks](pagelinks.md)|Links para abrir a página. O link `oneNoteClientURL` abre a página no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebUrl` abre a página no OneNote Online. Somente leitura.|
|ordem|Int32|A ordem da página dentro da seção pai dela. Somente leitura.|
|self|String|O ponto de extremidade onde você pode obter detalhes sobre a página. Somente leitura.|
|title|String|O título da página. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|O bloco de anotações que contém a página.  Somente leitura.|
|parentSection|[Section](section.md)|A seção que contém a página. Somente leitura.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get page](../api/page-get.md) | [Página](page.md) |Leia as propriedades e as relações da página.|
|[Atualizar o conteúdo da página](../api/page-update.md) | None |Atualizar o conteúdo HTML da página. |
|[Excluir página](../api/page-delete.md) | None |Exclua a página. |
|[copyToSection](../api/page-copytosection.md)| None |Copia a página para uma seção específica.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->