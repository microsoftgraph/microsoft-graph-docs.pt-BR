# <a name="organization-resource-type"></a>tipo de recurso organization

Representa um locatário do Azure Active Directory. Somente as operações de leitura e atualização têm suporte em locatários; criar e excluir não têm suporte. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter organização](../api/organization_get.md) | [organization](organization.md) |Leia as propriedades e as relações do objeto de organização.|
|[Update](../api/organization_update.md) | [organization](organization.md)  |Atualize o objeto organization. (Somente as propriedades **marketingNotificationMails** e **technicalNotificationMails** podem ser atualizadas.) |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Crie uma definição para a extensão de esquema e use-a para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

| Propriedade                             | Tipo                                                              | Descrição                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | Coleção [assignedPlan](assignedplan.md)                        | A coleção de planos de serviço associados ao locatário. Não anulável.                                                                                                                                                                                                            |
| cidade                                 | String                                                            |                                                                                                                                                                                                                                                                                      |
| companyLastDirSyncTime               | DateTimeOffset                                                    | A hora e a data em que o locatário foi sincronizado pela última vez com o diretório local. O tipo de Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` |
| country                              | String                                                            |                                                                                                                                                                                                                                                                                      |
| countryLetterCode                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| deletionTimestamp                    | DateTimeOffset                                                    | O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Booliano                                                           | **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).                        |
| displayName                          | String                                                            | O nome de exibição do locatário.                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | O identificador exclusivo do locatário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.                                                                                                                                                            |
| marketingNotificationEmails          | Coleção de cadeias de caracteres                                                 | Não anulável.                                                                                                                                                                                                                                                                        |
| objectType                           | String                                                            | Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é sempre "Empresa".                                                                                                                                                                                                 |
| postalCode                           | String                                                            |                                                                                                                                                                                                                                                                                      |
| preferredLanguage                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| provisionedPlans                     | Coleção [ProvisionedPlan](provisionedplan.md)                  | Não anulável.                                                                                                                                                                                                                                                                        |
| provisioningErrors                   | Coleção ProvisioningError | Não anulável.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | Coleção de cadeias de caracteres                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | Coleção de cadeias de caracteres                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String                                                            |                                                                                                                                                                                                                                                                                      |
| street                               | String                                                            |                                                                                                                                                                                                                                                                                      |
| technicalNotificationMails           | Coleção de cadeias de caracteres                                                 | Não anulável.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | String                                                            |                                                                                                                                                                                                                                                                                      |
| verifiedDomains                      | Coleção [VerifiedDomain](verifieddomain.md)                    | A coleção de domínios associados a este locatário. Não anulável.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para a organização. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>Veja também

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
  "tocPath": ""
}-->
