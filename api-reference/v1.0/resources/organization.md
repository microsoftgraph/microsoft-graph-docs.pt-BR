# <a name="organization-resource-type"></a>tipo de recurso organization

Representa um locatário do Azure Active Directory. Somente as operações de leitura e atualização têm suporte em locatários; criar e excluir não têm suporte. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter organização](../api/organization_get.md) | [organization](organization.md) |Leia as propriedades e as relações do objeto de organização.|
|[Update](../api/organization_update.md) | [organization](organization.md)  |Atualize o objeto organization. As únicas propriedades que podem ser atualizadas são: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** e **privacyProfile**. |
|**Extensões abertas**| | ||**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

| Propriedade                             | Tipo                                                              | Descrição                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | Coleção [assignedPlan](assignedplan.md)                        | A coleção de planos de serviço associados ao locatário. Não anulável.                                                                                                                                                                                                            |
| city                                 | Sequência de caracteres                                                            | Nome da cidade do endereço da organização                                                                                                                                                                                                                                        |
| companyLastDirSyncTime               | DateTimeOffset                                                    | A hora e a data em que o locatário foi sincronizado pela última vez com o diretório local. O tipo de Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` |
| country                              | Sequência de caracteres                                                            | Nome do país/região do endereço da organização                                                                                                                                                                                                                              |
| countryLetterCode                    | Sequência de caracteres                                                            | Abreviação de país/região da organização                                                                                                                                                                                                                                     |
| deletionTimestamp                    | DateTimeOffset                                                    | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Booleano                                                           | **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).                        |
| displayName                          | Sequência de caracteres                                                            | O nome de exibição do locatário.                                                                                                                                                                                                                                                     |
| id                                   | Sequência de caracteres                                                            | O identificador exclusivo do locatário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.                                                                                                                                                            |
| marketingNotificationEmails          | Coleção de cadeias de caracteres                                                 | Não anulável.                                                                                                                                                                                                                                                                        |
| objectType                           | Sequência de caracteres                                                            | Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é sempre "Empresa".                                                                                                                                                                                                 |
| postalCode                           | Sequência de caracteres                                                            | CEP do endereço da organização                                                                                                                                                                                                                                      |
| preferredLanguage                    | Sequência de caracteres                                                            | O idioma preferencial da organização. Deve seguir o código ISO 639-1; por exemplo "en".                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | O perfil de privacidade de uma organização.                                                                                                                                                                                                                                              |
| provisionedPlans                     | Coleção [ProvisionedPlan](provisionedplan.md)                  | Não anulável.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | Coleção de cadeias de caracteres                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | Coleção de cadeias de caracteres                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | Sequência de caracteres                                                            | Nome do estado do endereço da organização                                                                                                                                                                                                                                       |
| street                               | Sequência de caracteres                                                            | Nome da rua do endereço da organização                                                                                                                                                                                                                                          |
| technicalNotificationMails           | Coleção de cadeias de caracteres                                                 | Não anulável.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | Sequência de caracteres                                                            | Número de telefone da organização                                                                                                                                                                                                                                                |
| verifiedDomains                      | Coleção [VerifiedDomain](verifieddomain.md)                    | A coleção de domínios associados a este locatário. Não anulável.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para a organização. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "companyLastDirSyncTime": "2018-05-12T13:09:20.111Z",
  "country": "string",
  "countryLetterCode": "string",
  "deletionTimestamp": "2018-05-12T15:37:52.763Z",
  "dirSyncEnabled": true,
  "displayName": "string",
  "id": "string (identifier)",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "telephoneNumber": "555-555-6568",
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
