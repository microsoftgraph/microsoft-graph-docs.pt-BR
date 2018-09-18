# <a name="contact-resource-type"></a>tipo de recurso contact

Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).
- Inscrever-se para receber [notificações de alteração](../../../concepts/webhooks.md).
- Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais por meio de uma função [delta](../api/contact_delta.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contato](../api/contact_get.md) | [contact](contact.md) |Leia as propriedades e as relações do objeto contact.|
|[Create](../api/user_post_contacts.md) | [contact](contact.md) |Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.|
|[Update](../api/contact_update.md) | [contact](contact.md) |Atualize o objeto contact. |
|[Delete](../api/contact_delete.md) | Nenhuma |Exclua um objeto contact. |
|[delta](../api/contact_delta.md)|Coleção [Contact](contact.md)| Obtenha um conjunto de contatos que foram adicionados, excluídos ou atualizados em uma pasta especificada.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contact](contact.md)  |Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.   |
|[Obter contato com propriedade estendida com valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contact](contact.md) | Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.  |
|[Obter contato com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assistantName|Sequência de caracteres|O nome do assistente do contato.|
|birthday|DateTimeOffset|O aniversário do contato. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|businessAddress|[PhysicalAddress](physicaladdress.md)|O endereço comercial do contato.|
|businessHomePage|Sequência de caracteres|A home page comercial do contato.|
|businessPhones|Coleção de cadeias de caracteres|Os números de telefone comerciais do contato.|
|categories|Coleção de cadeias de caracteres|As categorias associadas ao contato.|
|changeKey|Sequência de caracteres|Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.|
|children|Coleção de cadeias de caracteres|Os nomes dos filhos do contato.|
|nomeDaEmpresa|Sequência de caracteres|O nome da empresa do contato.|
|createdDateTime|DateTimeOffset|A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|department|Sequência de caracteres|O departamento do contato.|
|displayName|Sequência de caracteres|O nome para exibição do contato.|
|emailAddresses|Coleção [EmailAddress](emailaddress.md)|Os endereços de email do contato.|
|sinalizar|[followUpFlag](followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|fileAs|Sequência de caracteres|O nome com o qual o contato está arquivado.|
|generation|Sequência de caracteres|A geração do contato.|
|givenName|Sequência de caracteres|O nome do contato.|
|homeAddress|[PhysicalAddress](physicaladdress.md)|O endereço residencial do contato.|
|homePhones|Coleção de cadeias de caracteres|Os números de telefone residenciais do contato.|
|id|Sequência de caracteres|O identificador exclusivo do contato. Somente leitura.|
|imAddresses|Coleção de cadeias de caracteres|Os endereços de mensagens instantâneas do contato.|
|initials|Sequência de caracteres|As iniciais do contato.|
|jobTitle|Sequência de caracteres|O cargo do contato.|
|lastModifiedDateTime|DateTimeOffset|A hora em que o contato foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|manager|Sequência de caracteres|O nome do gerente do contato.
|middleName|Sequência de caracteres|O nome do meio do contato.|
|mobilePhone|Sequência de caracteres|O número de celular do contato.|
|nickName|Sequência de caracteres|O apelido do contato.|
|officeLocation|Sequência de caracteres|O local do escritório do contato.|
|otherAddress|[PhysicalAddress](physicaladdress.md)|Outros endereços do contato.|
|parentFolderId|Sequência de caracteres|A ID da pasta pai do contato.|
|personalNotes|Sequência de caracteres|As anotações do usuário sobre o contato.|
|profession|Sequência de caracteres|A profissão do contato.|
|spouseName|Sequência de caracteres|O nome do cônjuge/parceiro do contato.|
|surname|Sequência de caracteres|O sobrenome do contato.|
|title|Sequência de caracteres|O título do contato.|
|yomiCompanyName|Sequência de caracteres|O nome de empresa japonês fonético do contato.|
|yomiGivenName|Sequência de caracteres|O nome japonês fonético do contato.|
|yomiSurname|Sequência de caracteres|O sobrenome japonês fonético do contato.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o contato. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.|
|Foto|[profilePhoto](profilephoto.md)| Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md)
- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
