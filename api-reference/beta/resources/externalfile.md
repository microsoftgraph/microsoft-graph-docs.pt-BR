---
title: Tipo de recurso externalFile
description: Um arquivo indexado por meio de uma conexão de Pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64b672c5f97a4093b1498c93f4402d49ff3ba417
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722021"
---
# <a name="externalfile-resource-type"></a>Tipo de recurso externalFile

Namespace: microsoft.graph

> [!CAUTION]
> O `externalFile` tipo foi preterido. Os desenvolvedores não devem usar esse tipo. Os arquivos externos ainda podem ser indexados usando o [tipo externalItem.](externalitem.md)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um item indexado por meio de uma conexão de Pesquisa [da](externalconnection.md)Microsoft . Esse tipo deriva do [tipo externalItem.](externalitem.md)

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método                                                        | Tipo de retorno  | Descrição |
|:--------------------------------------------------------------|:-------------|:--|
| [Criar externalFile](../api/externalconnection-put-items.md) | externalFile | Crie um externalFile. |
| [Atualizar externalFile](../api/externalitem-update.md)          | externalFile | Atualize um externalFile. |
| [Delete](../api/externalitem-delete.md)                       | Nenhum(a)         | Exclua um externalFile. |

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                     | Descrição                    |
|:-----------------|:-------------------------|:-------------------------------|
| acl              | [Coleção acl](acl.md) | Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. Obrigatório. |
| content          | Cadeia de caracteres                   | Uma representação em texto sem texto do conteúdo do item. O texto nesta propriedade é indexado em texto completo. Opcional. |
| id               | Cadeia de caracteres                   | ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md). Deve ser alfanumérico e um máximo de 128 caracteres. Obrigatório. |
| createdBy        | Cadeia de caracteres                   | O nome do usuário que criou o arquivo. |
| createdDateTime  | DateTimeOffset           | A data e a hora em que o arquivo foi criado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z` |
| extension        | Cadeia de caracteres                   | A extensão de arquivo.            |
| lastModifiedBy   | Cadeia de caracteres                   | O nome do usuário que modificou o arquivo pela última vez. |
| modifiedDateTime | DateTimeOffset           | A data e a hora em que o arquivo foi modificado pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z` |
| nome             | Cadeia de caracteres                   | O nome do arquivo. Obrigatório.       |
| size             | Int64                    | O tamanho do arquivo em bytes. |
| title            | Cadeia de caracteres                   | O título do arquivo.         |
| url              | Cadeia de caracteres                   | A URL para acessar o arquivo. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


