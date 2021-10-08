---
title: tipo de recurso organization
description: 'Representa um locatário do Azure Active Directory. '
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f3a07629006f5f2cada6601dab09b952fdef7980
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240758"
---
# <a name="organization-resource-type"></a>tipo de recurso organization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o locatário do Azure Active Directory conectado ao usuário ou aplicativo. Somente as operações de leitura e atualização têm suporte nesses recursos; criar e excluir não têm suporte. Herda de [directoryObject](directoryobject.md).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter organização](../api/organization-get.md) | Coleção [organization](organization.md)|Leia as propriedades e as relações do objeto de organização.|
|[Atualizar a organização](../api/organization-update.md) | [organization](organization.md)  |Atualize o objeto organization. As únicas propriedades que podem ser atualizadas são: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** e **privacyProfile**. |
| [Obter configurações da organização](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Leia o objeto de configurações da organização. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../api/schemaextension-post-schemaextensions.md) | [schemaExtension](schemaextension.md) | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Licenças da organização**| | |
|[activateService](../api/organization-activateservice.md) | Nenhum |  Ative um serviço para uma organização. |
|**Identidade visual organizacional**| | |
|[Obter organizationalBranding](../api/organizationalbranding-get.md) | [organizationalBranding](organizationalbranding.md) | Obtenha o objeto de identidade visual organizacional padrão. |
|[Atualizar organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Atualize o objeto de identidade visual organizacional padrão. |
|[Criar organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Crie uma nova identidade visual de localização (específica do idioma) e um objeto de identidade visual padrão, caso não exista. |
|[Listar organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | coleção [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Recupere todos os objetos de identidade visual de localização no locatário. |
|[Obter organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Leia as propriedades de um objeto de identidade visual de localização. |
|[Atualizar organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Atualize um objeto de identidade visual de localização. |
|[Excluir organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Exclua um objeto de identidade visual de localização. |
<!--|[Excluir organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Exclua o objeto de identidade visual organizacional padrão. |

**OBSERVAÇÃO: para restaurar a operação Excluir organizationalBranding de volta à tabela após Atualizar organizationalBranding se todas as inconsistências são resolvidas.-->

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| assignedPlans | Coleção [assignedPlan](assignedplan.md) | A coleção de planos de serviço associados ao locatário. Não anulável. |
| businessPhones | Coleção de cadeias de caracteres | Número de telefone para a organização. Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade. |
| city | Cadeia de caracteres | Nome da cidade do endereço da organização. |
| country | Cadeia de caracteres | Nome do país/região do endereço da organização. |
| countryLetterCode | Cadeia de caracteres | Abreviação do país/região da organização. |
| createdDateTime | DateTimeOffset | Carimbo de hora de criação da organização. Não é possível modificar o valor e ele é preenchido automaticamente quando a organização é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| deletedDateTime | DateTimeOffset | Representa a data e a hora que o locatário do Azure AD foi excluído usando o formato ISO 8601 e está sempre no horário do UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| directorySizeQuota | [directorySizeQuota](directorySizeQuota.md) | As informações de cota de tamanho do diretório de uma organização. |
| displayName | String | O nome de exibição do locatário. |
| id | Cadeia de caracteres | A ID do locatário, um identificador exclusivo que representa a organização (ou Locatário). Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| isMultipleDataLocationsForServicesEnabled | Boolean | `true` se a organização estiver habilitada para Multi-Geo; `false` se a organização não estiver habilitada para Multi-Geo; `null` (padrão). Somente leitura. Para saber mais, confira [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction). |
| marketingNotificationEmails | Coleção de cadeias de caracteres | Não anulável. |
| objectType | String | Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é `Company` sempre .|
| onPremisesLastSyncDateTime | DateTimeOffset | A hora e a data em que o locatário foi sincronizado pela última vez com o diretório no local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
| onPremisesSyncEnabled | Booliano | `true` se esse objeto for sincronizado de um diretório local; se esse objeto foi originalmente sincronizado de um diretório local, mas `false` não está mais sincronizado; Anulavel. `null` se este objeto nunca foi sincronizado de um diretório local (padrão). |
| postalCode | Cadeia de caracteres | CEP do endereço da organização. |
| preferredLanguage | String | O idioma preferencial da organização. Deve seguir o Código ISO 639-1; por exemplo `en`. |
| privacyProfile | [privacyProfile](privacyprofile.md) | O perfil de privacidade de uma organização. |
| provisionedPlans | coleção [provisionedPlan](provisionedplan.md) | Não anulável. |
| securityComplianceNotificationMails | Coleção de cadeias de caracteres ||
| securityComplianceNotificationPhones | Coleção de cadeias de caracteres ||
| state | Cadeia de caracteres | Nome do estado do endereço da organização. |
| street | Cadeia de caracteres | Nome da rua do endereço da organização. |
| technicalNotificationMails |Coleção de cadeias de caracteres | Não anulável. |
| verifiedDomains | [coleção verifiedDomain](verifieddomain.md)|A coleção de domínios associados a este locatário. Não anulável. |

## <a name="relationships"></a>Relações

| Relação  | Tipo  |Descrição|
|:---------------|:--------|:----------|
|certificateBasedAuthConfiguration|coleção [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md)| Propriedade de navegação para gerenciar a configuração de autenticação baseada em certificado. Somente uma única instância de certificateBasedAuthConfiguration pode ser criada na coleção.  |
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o recurso da organização. Anulável.| 
|organizationalBranding|coleção [organizationalBranding](organizationalbranding.md)| Recurso para gerenciar a identidade visual padrão da organização. Anulável.|
|settings|[organizationSettings](organizationsettings.md) | Recupere as propriedades e as relações do objeto organizationSettings. Anulável.|

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
  "businessPhones": ["String"],
  "city": "String",
  "country": "String",
  "countryLetterCode": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
  "displayName": "String",
  "id": "String (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "marketingNotificationEmails": ["String"],
  "objectType": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["String"],
  "securityComplianceNotificationPhones": ["String"],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": ["String"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
