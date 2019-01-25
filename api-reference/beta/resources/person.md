---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa em email, contatos e redes sociais. Pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (por exemplo, email e Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512399"
---
# <a name="person-resource-type"></a>Tipo de recurso person

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma agregação de informações sobre uma pessoa em email, contatos e redes sociais. Pessoas podem ser contatos locais, contatos de redes sociais, diretório da sua organização e pessoas de comunicações recentes (por exemplo, email e Skype).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar pessoas](../api/user-list-people.md) | **person** |Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|birthday|string|O aniversário da pessoa.|
|companyName|string|O nome da empresa da pessoa.|
|departamento|string|O departamento da pessoa.|
|displayName|string|O nome de exibição da pessoa.|
|emailAddresses|coleção [rankedEmailAddress](rankedemailaddress.md)|Os endereços de email da pessoa.|
|givenName|string|O nome fornecido da pessoa.|
|id|string|O identificador exclusivo da pessoa. Somente leitura.|
|isFavorite|booliano|`true` se o usuário tiver sinalizado essa pessoa como um favorito.|
|MailboxType|string|O tipo de caixa de correio que é representado por um endereço de email da pessoa.|
|officeLocation|string|O local do escritório da pessoa.|
|personNotes|string|As anotações de forma livre que o usuário fez sobre essa pessoa.|
|personType|string|O tipo da pessoa, por exemplo lista de distribuição.|
|telefones|Coleção [phone](phone.md)|Os números de telefone da pessoa.|
|postalAddresses|[location](location.md) collection|Os endereços da pessoa.|
|profession|string|A profissão da pessoa.|
|sources|coleção [personDataSource](persondatasource.md)|As fontes de dados do usuário provêm, por exemplo, diretório ou contatos do Outlook.|
|surname|string|O sobrenome da pessoa.|
|title|string|Título da pessoa.|
|userPrincipalName|string|O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.|
|websites|Coleção [website](website.md)|Os sites da pessoa.|
|yomiCompany|string|O nome japonês fonético da empresa da pessoa.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/person.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
