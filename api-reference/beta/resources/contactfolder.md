---
title: tipo de recurso contactFolder
description: Uma pasta que contém contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a4fcb5152a3d7cb5f26214cf2b0a1e4a31dc1ffb
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575867"
---
# <a name="contactfolder-resource-type"></a>tipo de recurso contactFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma pasta que contém contatos.

Esse recurso suporta a utilização da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contactfolder-delta.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contactFolder](../api/contactfolder-get.md) | [contactFolder](contactfolder.md) |Obtenha uma pasta de contatos usando a respectiva ID.|
|[Update](../api/contactfolder-update.md) | [contactFolder](contactfolder.md) |Atualize o objeto contactFolder. |
|[Delete](../api/contactfolder-delete.md) | Nenhuma |Exclua um objeto contactFolder. |
|[Listar childFolders](../api/contactfolder-list-childfolders.md) |coleção [contactFolder](contactfolder.md)| Obtenha uma coleção de pastas filho sob a pasta de contatos especificada.|
|[Criar contactFolder filho](../api/contactfolder-post-childfolders.md) |[contactFolder](contactfolder.md)| Crie uma nova contactFolder como um filho de uma pasta especificada.|
|[delta](../api/contact-delta.md)|Coleção [Contact](contact.md)| Obtenha um conjunto de pastas de contatos que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.|
|[Listar contatos na pasta](../api/contactfolder-list-contacts.md) |Coleção [Contact](contact.md)| Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.|
|[Criar contato na pasta](../api/contactfolder-post-contacts.md) |[contato](contact.md)| Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contactFolder](contactfolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma contactFolder nova ou existente.   |
|[Obter contactFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Obtenha contactFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contactFolder](contactfolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma contactFolder nova ou existente.  |
|[Obter contactFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Obtenha uma contactFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|O nome de exibição da pasta.|
|id|String|Identificador exclusivo da pasta de contatos. Somente leitura.|
|parentFolderId|String|A ID da pasta pai da pasta.|
|wellKnownName|string|O nome da pasta se a pasta for uma pasta reconhecida. No momento `contacts` é a única pasta Contatos reconhecidas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|childFolders|Coleção [ContactFolder](contactfolder.md)|A coleção de pastas filho na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos na pasta. Propriedade de navegação. Somente leitura. Anulável.|
|multiValueLegacyExtendedProperty|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|
|singleValueLegacyExtendedProperty|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a contactFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
