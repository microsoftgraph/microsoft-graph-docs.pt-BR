# <a name="person-resource-type"></a>Tipo de recurso person

Uma agregação de informações sobre uma pessoa provenientes de emails, contatos e redes sociais. As pessoas podem ser contatos locais, contatos das redes sociais ou do diretório da sua organização e as pessoas de comunicações recentes (como emails e Skype).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar pessoas](../api/user_list_people.md) | **person** |Obtém uma coleção de objetos person ordenados por relevância para o [usuário](../resources/user.md).|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|birthday|Sequência de caracteres|O aniversário da pessoa.|
|companyName|Sequência de caracteres|O nome da empresa da pessoa.|
|departamento|Sequência de caracteres|O departamento da pessoa.|
|displayName|Sequência de caracteres|O nome de exibição da pessoa.|
|scoredEmailAddresses|Coleção [scoredEmailAddress](scoredemailaddress.md)|Os endereços de email da pessoa.|
|givenName|Sequência de caracteres|O nome fornecido da pessoa.|
|id|Sequência de caracteres|O identificador exclusivo da pessoa. Somente leitura.|
|imAddress|Cadeia de caracteres|O endereço do protocolo SIP (Início de Sessão) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.|
|isFavorite|Booleano|`true` se o usuário tiver sinalizado essa pessoa como um favorito.|
|jobTitle|Sequência de caracteres|O cargo da pessoa.|
|officeLocation|Sequência de caracteres|O local do escritório da pessoa.|
|personNotes|Cadeia de caracteres|As anotações de forma livre que o usuário fez sobre essa pessoa.|
|personType|[personType](persontype.md) |O tipo de pessoa.|
|telefones|Coleção [phone](phone.md)|Os números de telefone da pessoa.|
|postalAddresses|Coleção [location](location.md)|Os endereços da pessoa.|
|profession|Sequência de caracteres|A profissão da pessoa.|
|surname|Sequência de caracteres|O sobrenome da pessoa.|
|userPrincipalName|Sequência de caracteres|O nome UPN da pessoa. O UPN é um nome de logon para a pessoa ao estilo da Internet com base na [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email da pessoa. O formato geral é alias@domínio.|
|websites|Coleção [website](website.md)|Os sites da pessoa.|
|yomiCompany|Sequência de caracteres|O nome japonês fonético da empresa da pessoa.|

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
