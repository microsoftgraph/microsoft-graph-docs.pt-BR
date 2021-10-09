---
title: tipo de recurso organization
description: " criar e excluir não têm suporte. Herda de directoryObject."
ms.localizationpriority: high
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2b4ac86a3dd1bad876c6819b9f49c28ca4bac7fb
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240884"
---
# <a name="organization-resource-type"></a>tipo de recurso organization

Namespace: microsoft.graph

Representa o locatário do Azure Active Directory conectado ao usuário ou aplicativo. Somente as operações de leitura e atualização têm suporte nesses recursos; criar e excluir não têm suporte. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter organização](../api/organization-get.md) | Coleção [organization](organization.md)|Leia as propriedades e as relações do objeto de organização.|
|[Update](../api/organization-update.md) | [organization](organization.md)  |Atualizar o objeto da organização. As únicas propriedades que podem ser atualizadas são: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** e **privacyProfile**. |
|**Extensões abertas**| 
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| 
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Identidade visual organizacional**| | |
|[Obter organizationalBranding](../api/organizationalbranding-get.md) | [organizationalBranding](organizationalbranding.md) | Obtenha o objeto de identidade visual organizacional padrão. |
|[Atualizar organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Atualize o objeto de identidade visual organizacional padrão. |
|[Criar organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Crie uma nova identidade visual de localização (específica do idioma) e um objeto de identidade visual padrão, caso não exista. |
|[Listar organizationalBrandingLocalization](../api/organizationalbranding-list-localizations.md) | coleção [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Recupere todos os objetos de identidade visual de localização no locatário. |
|[Obter organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Leia as propriedades de um objeto de identidade visual de localização. |
|[Atualizar organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Atualize um objeto de identidade visual de localização. |
|[Excluir organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Exclua um objeto de identidade visual de localização. |
<!--|[Excluir organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Exclua o objeto de identidade visual organizacional padrão. |

** OBSERVAÇÃO: para restaurar a operação Excluir organizationalBranding na tabela após Atualizar organizationalBranding se todas as inconsistências forem resolvidas.-->

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| assignedPlans | Coleção [assignedPlan](assignedplan.md) | A coleção de planos de serviço associados ao locatário. Não anulável. |
| businessPhones | Coleção de cadeias de caracteres | Número de telefone para a organização. Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade. |
| city | Cadeia de caracteres | Nome da cidade do endereço da organização. |
| country | Cadeia de caracteres | Nome do país/região do endereço da organização. |
| countryLetterCode | Cadeia de caracteres | Abreviação do país/região da organização. |
| createdDateTime | DateTimeOffset | Carimbo de hora de criação da organização. Não é possível modificar o valor e ele é preenchido automaticamente quando a organização é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| deletedDateTime | DateTimeOffset | Representa a data e hora em que o locatário do Azure AD foi excluído usando o formato ISO 8601 e está sempre no fuso UTC. Por exemplo, meia-noite UTC do dia 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| displayName | String | O nome de exibição do locatário. |
| id | Cadeia de caracteres | A ID do locatário, um identificador exclusivo que representa a organização (ou Locatário). Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| isMultipleDataLocationsForServicesEnabled | Boolean | `true` se a organização estiver habilitada para Multi-Geo; **fallse** se a organização não estiver habilitada para Multi-Geo; **null** (padrão). Somente leitura. Para saber mais, confira [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction). |
| marketingNotificationEmails | Coleção de cadeias de caracteres | Não anulável. |
| onPremisesLastSyncDateTime | DateTimeOffset | A data e hora em que o locatário foi sincronizado com o diretório no local pela última vez. O tipo de carimbo de data/hora apresenta as informações de data e hora usando o formato ISO 8601 e está sempre no fuso UTC. Por exemplo, meia-noite UTC do dia 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
| onPremisesSyncEnabled | Booliano | `true` se esse objeto estiver sendo sincronizado a partir de um diretório local; `false` se, originalmente, esse objeto era sincronizado a partir de um diretório local, mas não está mais sendo sincronizado; `null` se esse objeto nunca foi sincronizado a partir de um diretório local (padrão). |
| postalCode | Cadeia de caracteres | CEP do endereço da organização. |
| preferredLanguage | Cadeia de caracteres | Idioma preferencial da organização. Deve seguir o Código ISO 639-1; por exemplo, `en`. |
| privacyProfile | [privacyProfile](privacyprofile.md) | O perfil de privacidade de uma organização. |
| provisionedPlans | Coleção [ProvisionedPlan](provisionedplan.md) | Não anulável. |
| securityComplianceNotificationMails | Coleção de cadeias de caracteres ||
| securityComplianceNotificationPhones | Coleção de cadeias de caracteres||
| state | Cadeia de caracteres | Nome do estado do endereço da organização. |
| street | Cadeia de caracteres | Nome da rua do endereço da organização. |
| technicalNotificationMails | Coleção de cadeias de caracteres | Não anulável. |
| verifiedDomains | Coleção [VerifiedDomain](verifieddomain.md) | A coleção de domínios associados a este locatário. Não anulável. |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|certificateBasedAuthConfiguration|coleção [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md)| Propriedade de navegação para gerenciar a configuração de autenticação baseada em certificado. Somente uma única instância de certificateBasedAuthConfiguration pode ser criada na coleção.  |
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para a organização. Somente leitura. Anulável.|
|organizationalBranding|coleção [organizationalBranding](organizationalbranding.md)| Identidade visual da organização. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
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
  "suppressions": [
  ],
  "tocPath": ""
}-->
