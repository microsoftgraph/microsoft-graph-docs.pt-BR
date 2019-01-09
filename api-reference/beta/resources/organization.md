---
title: tipo de recurso organization
description: 'Representa um locatário do Azure Active Directory. '
ms.openlocfilehash: 2e9a9a32411164e270e2eb3a8830fa811ba5f9cb
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771825"
---
# <a name="organization-resource-type"></a>tipo de recurso organization

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o locatário do Azure Active Directory que o usuário ou aplicativo está conectado ao. Somente as operações de leitura e a atualização são suportadas neste recurso; criar e excluir não são suportados. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter organização](../api/organization-get.md) | [organization](organization.md) |Leia as propriedades e as relações do objeto de organização.|
|[Update](../api/organization-update.md) | [organization](organization.md)  |Atualize o objeto organization. As únicas propriedades que podem ser atualizadas são: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** e **privacyProfile**. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|A coleção de planos de serviço associados ao locatário. Não anulável.            |
| businessPhones                      | String collection                                         | Número de telefone para a organização. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.                                                                                            |
|city|String| Nome da cidade do endereço da organização |
|companyLastDirSyncTime|DateTimeOffset|A hora e a data em que o locatário foi sincronizado pela última vez com o diretório local. O tipo de Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|country|String| Nome do país/região do endereço da organização |
|countryLetterCode|String| Abreviação de país/região da organização |
|createdDateTime|DateTimeOffset| Carimbo de hora de quando a organização foi criada. O valor não pode ser modificado e é preenchido automaticamente quando a organização é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
| deletedDateTime                    | DateTimeOffset                                                    | Representa a data e hora de quando o locatário do Azure AD foi excluído, usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.                                                                                     |
|dirSyncEnabled|Booliano|**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão).|
|displayName|String|O nome de exibição do locatário.|
|id|String|A ID do inquilino, um identificador exclusivo que representa a organização (ou Locatário). Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|isMultipleDataLocationsForServicesEnabled|Booliano|**true** se a organização estiver habilitada; Multi-Geo **false** se a organização não estiver habilitado Multi-Geo; **Nulo** (padrão). Somente leitura. Para obter mais informações, consulte [Multi-Geo OneDrive Online](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|marketingNotificationEmails|Coleção de cadeias de caracteres| Não anulável.            |
|objectType|String|Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é sempre "Empresa". |
|postalCode|String| CEP do endereço da organização |
|preferredLanguage|String| O idioma preferencial da organização. Deve seguir o código ISO 639-1; por exemplo "en". |
|privacyProfile|[privacyProfile](privacyprofile.md)| O perfil de privacidade de uma organização.            |
|provisionedPlans|Coleção [ProvisionedPlan](provisionedplan.md)| Não anulável.            |
|provisioningErrors|Coleção ProvisioningError| Não anulável.            |
|securityComplianceNotificationMails|Coleção de cadeias de caracteres||
|securityComplianceNotificationPhones|Coleção de cadeias de caracteres||
|state|String| Nome do estado do endereço da organização |
|street|String| Nome da rua do endereço da organização |
|technicalNotificationMails|Coleção de cadeias de caracteres| Não anulável. |
|verifiedDomains|Coleção [VerifiedDomain](verifieddomain.md)|A coleção de domínios associados a este locatário. Não anulável.            |

## <a name="relationships"></a>Relações

| Relação     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões open definido para o recurso de organização. Anulável.|

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
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
