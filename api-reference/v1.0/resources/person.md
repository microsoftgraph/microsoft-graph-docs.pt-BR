---
title: Tipo de recurso person
description: Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 33e177875c7e7724659df79d191c2fe07bc1a2a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117799"
---
# <a name="person-resource-type"></a>Tipo de recurso person

Namespace: microsoft.graph

Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar pessoas](../api/user-list-people.md) | **person** |Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|birthday|String|O aniversário da pessoa.|
|companyName|String|O nome da empresa da pessoa.|
|departamento|String|O departamento da pessoa.|
|displayName|String|O nome de exibição da pessoa.|
|scoredEmailAddresses|Coleção [scoredEmailAddress](scoredemailaddress.md)|Os endereços de email da pessoa.|
|givenName|String|O nome fornecido da pessoa.|
|id|String|O identificador exclusivo da pessoa. Somente leitura.|
|imAddress|String|O endereço do protocolo SIP (Início de Sessão) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.|
|isFavorite|Boolean|`true` se o usuário tiver sinalizado essa pessoa como um favorito.|
|jobTitle|String|O cargo da pessoa.|
|officeLocation|String|O local do escritório da pessoa.|
|personNotes|String|As anotações de forma livre que o usuário fez sobre essa pessoa.|
|personType|[personType](persontype.md) |O tipo de pessoa.|
|telefones|Coleção [phone](phone.md)|Os números de telefone da pessoa.|
|postalAddresses|[location](location.md) collection|Os endereços da pessoa.|
|profession|String|A profissão da pessoa.|
|surname|String|O sobrenome da pessoa.|
|userPrincipalName|String|O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.|
|websites|Coleção [website](website.md)|Os sites da pessoa.|
|yomiCompany|String|O nome japonês fonético da empresa da pessoa.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

