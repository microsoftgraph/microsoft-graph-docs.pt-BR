---
title: tipo de recurso contact
description: Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d2bdc1be9e504bc72ce12ffe924b6da0812b99ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513575"
---
# <a name="contact-resource-type"></a>tipo de recurso contact

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/contact-delta.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assistantName|String|O nome do assistente do contato.|
|birthday|DateTimeOffset|O aniversário do contato. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|categories|Coleção String|As categorias associadas ao contato. Cada categoria corresponde à propriedade **displayName** de um [outlookCategory](outlookcategory.md) definidas para o usuário.|
|changeKey|String|Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.|
|children|String collection|Os nomes dos filhos do contato.|
|nomeDaEmpresa|String|O nome da empresa do contato.|
|createdDateTime|DateTimeOffset|A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|department|String|O departamento do contato.|
|displayName|String|O nome para exibição do contato. Você pode especificar o nome para exibição em uma operação de [criar](../api/user-post-contacts.md) ou [Atualizar](../api/contact-update.md) . Observe que as atualizações posteriores a outras propriedades podem causar um valor gerado automaticamente substituir o valor displayName que você especificou. Para preservar a um valor pré-existente, sempre incluí-lo como displayName em uma operação de [atualização](../api/contact-update.md) .|
|emailAddresses|coleção [typedEmailAddress](typedemailaddress.md)|Os endereços de email do contato.|
|fileAs|String|O nome com o qual o contato está arquivado.|
|sinalizar|[followUpFlag](followupflag.md)|O valor de sinalizador que indica o status, data de início, data de conclusão ou data de conclusão do contato. |
|gender |String |Gênero do contato. |
|generation|String|A geração do contato.|
|givenName|String|O nome do contato.|
|id|String|O identificador exclusivo do contato. Somente leitura.|
|imAddresses|Coleção de cadeias de caracteres|Os endereços de mensagens instantâneas do contato.|
|initials|String|As iniciais do contato.|
|jobTitle|String|O cargo do contato.|
|lastModifiedDateTime|DateTimeOffset|A hora em que o contato foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|manager|String|O nome do gerente do contato.
|middleName|String|O nome do meio do contato.|
|nickName|String|O apelido do contato.|
|officeLocation|String|O local do escritório do contato.|
|parentFolderId|String|A ID da pasta pai do contato.|
|personalNotes|String|As anotações do usuário sobre o contato.|
|telefones |Coleção [phone](phone.md) |Números de telefone associados com o contato, por exemplo, telefone residencial, celular e telefone comercial. |
|postalAddresses |coleção [physicalAddress](physicaladdress.md) |Endereços associados ao contato, por exemplo, início endereço e o endereço comercial. |
|profession|String|A profissão do contato.|
|spouseName|String|O nome do cônjuge/parceiro do contato.|
|surname|Cadeia de caracteres|O sobrenome do contato.|
|title|Cadeia de caracteres|O título do contato.|
|websites |Coleção [website](website.md)|Sites da Web associados ao contato. |
|WeddingAnniversary |Data |Aniversário de chá do contato. |
|yomiCompanyName|String|O nome de empresa japonês fonético do contato.|
|yomiGivenName|String|O nome japonês fonético do contato.|
|yomiSurname|String|O sobrenome japonês fonético do contato.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões open definidas para o contato. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.|
|Foto|[photo](profilephoto.md)| Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.|

## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter contato](../api/contact-get.md) | [contato](contact.md) |Leia as propriedades e as relações do objeto contact.|
|[Create](../api/user-post-contacts.md) | [contato](contact.md) |Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.|
|[Update](../api/contact-update.md) | [contato](contact.md) |Atualize o objeto contact. |
|[Delete](../api/contact-delete.md) | Nenhuma |Exclua um objeto contact. |
|[delta](../api/contact-delta.md)|Coleção [Contact](contact.md)| Obtenha um conjunto de contatos que foram adicionados, excluídos ou atualizados em uma pasta especificada.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contato](contact.md)  |Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.   |
|[Obter contato com propriedade estendida com valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [contato](contact.md) | Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contato](contact.md) | Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.  |
|[Obter contato com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [contact](contact.md) | Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)
- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
