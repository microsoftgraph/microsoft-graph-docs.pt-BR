---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2501a97d21026ffe9cba907729822c2c72b0912b6ebfc20cb6591637089a2960
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184918"
---
# <a name="contactfolder-resource-type"></a>tipo de recurso contactFolder

Namespace: microsoft.graph

Uma pasta que contém contatos.

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contactFolder](../api/contactfolder-get.md) | [pastadeContatos](contactfolder.md) |Obtenha uma pasta de contatos usando a respectiva ID.|
|[Update](../api/contactfolder-update.md) | [pastadeContatos](contactfolder.md) |Atualize o objeto contactFolder. |
|[Delete](../api/contactfolder-delete.md) | None |Exclua um objeto contactFolder. |
|[Listar childFolders](../api/contactfolder-list-childfolders.md) |Coleção [ContactFolder](contactfolder.md)| Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.|
|[Criar contactFolder filho](../api/contactfolder-post-childfolders.md) |[ContactFolder](contactfolder.md)| Crie uma nova contactFolder como um filho de uma pasta especificada.|
|[delta](../api/contact-delta.md)|Coleção [Contact](contact.md)| Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.|
|[Listar contatos na pasta](../api/contactfolder-list-contacts.md) |Coleção [Contact](contact.md)| Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.|
|[Criar contato na pasta](../api/contactfolder-post-contacts.md) |[Contact](contact.md)| Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.|
|[Criar propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[pastadeContatos](contactfolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.   |
|[Obter contactFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [pastadeContatos](contactfolder.md) | Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [pastadeContatos](contactfolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.  |
|[Obter contactFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [pastadeContatos](contactfolder.md) | Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição da pasta.|
|id|Cadeia de caracteres|Identificador exclusivo da pasta de contatos. Somente leitura.|
|parentFolderId|String|A ID da pasta pai da pasta.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|childFolders|Coleção [ContactFolder](contactfolder.md)|A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

