---
title: tipo de recurso externalfile
description: Um arquivo indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a4f4e9bb9a782e71dd0c2f349baaacc5b61f480
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892594"
---
# <a name="externalfile-resource-type"></a>tipo de recurso externalfile

Namespace: microsoft.graph

> [!CAUTION]
> O `externalFile` tipo foi preterido. Os desenvolvedores não devem usar esse tipo. Arquivos externos ainda podem ser indexados usando o tipo [externalItem](externalitem.md) .

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft. Esse tipo deriva do tipo [externalItem](externalitem.md) .

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Methods

| Método                                                        | Tipo de retorno  | Descrição |
|:--------------------------------------------------------------|:-------------|:--|
| [Criar externalfile](../api/externalconnection-put-items.md) | externalFile | Criar um externalfile. |
| [Atualizar externalfile](../api/externalitem-update.md)          | externalFile | Atualize um externalfile. |
| [Delete](../api/externalitem-delete.md)                       | None         | Excluir um externalfile. |

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                     | Descrição                    |
|:-----------------|:-------------------------|:-------------------------------|
| ACL              | coleção [ACL](acl.md) | Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. Obrigatório. |
| content          | String                   | Uma representação de texto simples do conteúdo do item. O texto nessa propriedade é indexado de texto completo. Opcional. |
| id               | String                   | ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o. Deve ser alfanumérico e um máximo de 128 caracteres. Obrigatório. |
| createdBy        | String                   | O nome do usuário que criou o arquivo. |
| createdDateTime  | DateTimeOffset           | A data e hora em que o arquivo foi criado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` |
| extensões        | String                   | A extensão de arquivo.            |
| lastModifiedBy   | String                   | O nome do usuário que modificou o arquivo pela última vez. |
| modifiedDateTime | DateTimeOffset           | A data e hora em que o arquivo foi modificado pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` |
| nome             | Cadeia de caracteres                   | O nome do arquivo. Obrigatório.       |
| size             | Int64                    | O tamanho do arquivo em bytes. |
| title            | String                   | O título do arquivo.         |
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
