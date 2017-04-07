# <a name="contact-resource-type"></a>tipo de recurso contact

Um contato é um item no Outlook no qual você pode organizar e salvar informações sobre as pessoas e organizações com quem se comunica. Os contatos estão contidos em pastas de contatos.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter contato](../api/contact_get.md) | [contact](contact.md) |Leia as propriedades e as relações do objeto contact.|
|[Create](../api/user_post_contacts.md) | [contact](contact.md) |Adicione um contato na pasta de Contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.|
|[Update](../api/contact_update.md) | [contact](contact.md) |Atualize o objeto contact. |
|[Delete](../api/contact_delete.md) | Nenhuma |Exclua um objeto contact. |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contact](contact.md)  |Criar uma ou mais propriedades estendidas de valor único em um contato novo ou existente.   |
|[Obter contato com propriedade estendida com valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Obter contatos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contact](contact.md) | Criar uma ou mais propriedades estendidas de vários valores em um contato novo ou existente.  |
|[Obter contato com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [contact](contact.md) | Obter um contato que contenha uma propriedade estendida de vários valores usando `$expand`. |


## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|assistantName|String|O nome do assistente do contato.|
|birthday|DateTimeOffset|O aniversário do contato. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|businessAddress|[PhysicalAddress](physicaladdress.md)|O endereço comercial do contato.|
|businessHomePage|String|A home page comercial do contato.|
|businessPhones|Coleção de cadeias de caracteres|Os números de telefone comerciais do contato.|
|categories|Coleção de cadeias de caracteres|As categorias associadas ao contato.|
|changeKey|String|Identifica a versão do contato. Toda vez que o contato muda, a ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.|
|children|Coleção de cadeias de caracteres|Os nomes dos filhos do contato.|
|nomeDaEmpresa|String|O nome da empresa do contato.|
|createdDateTime|DateTimeOffset|A hora em que o contato foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|department|String|O departamento do contato.|
|displayName|String|O nome para exibição do contato.|
|emailAddresses|Coleção [EmailAddress](emailaddress.md)|Os endereços de email do contato.|
|fileAs|String|O nome com o qual o contato está arquivado.|
|generation|String|A geração do contato.|
|givenName|String|O nome do contato.|
|homeAddress|[PhysicalAddress](physicaladdress.md)|O endereço residencial do contato.|
|homePhones|Coleção de cadeias de caracteres|Os números de telefone residenciais do contato.|
|id|String|O identificador exclusivo do contato. Somente leitura.|
|imAddresses|Coleção de cadeias de caracteres|Os endereços de mensagens instantâneas do contato.|
|initials|String|As iniciais do contato.|
|jobTitle|String|O cargo do contato.|
|lastModifiedDateTime|DateTimeOffset|A hora em que o contato foi modificado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|manager|String|O nome do gerente do contato.
|middleName|String|O nome do meio do contato.|
|mobilePhone|String|O número de celular do contato.|
|nickName|String|O apelido do contato.|
|officeLocation|String|O local do escritório do contato.|
|otherAddress|[PhysicalAddress](physicaladdress.md)|Outros endereços do contato.|
|parentFolderId|String|A ID da pasta pai do contato.|
|personalNotes|String|As anotações do usuário sobre o contato.|
|profession|String|A profissão do contato.|
|spouseName|String|O nome do cônjuge do contato.|
|surname|String|O sobrenome do contato.|
|title|String|O título do contato.|
|yomiCompanyName|String|O nome de empresa japonês fonético do contato.|
|yomiGivenName|String|O nome japonês fonético do contato.|
|yomiSurname|String|O sobrenome japonês fonético do contato.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o contato. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para o contato. Somente leitura. Anulável.|
|Foto|[profilePhoto](profilephoto.md)| Imagem de contato opcional. Você pode obter ou definir uma foto de um contato.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para o contato. Somente leitura. Anulável.|


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
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
