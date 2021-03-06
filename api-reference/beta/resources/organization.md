---
title: tipo de recurso organization
description: 'Representa um locatário do Azure Active Directory. '
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ea21e90c720962c7fc047edd6f19630c3918b352
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721338"
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
|[Criar organizationalBrandingProperties](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Crie uma nova organizationalBrandingProperties postando na coleção de identidade visual. |
|[Obter identidade visual](../api/organizationalbrandingproperties-get.md) | [Coleção organizationalBrandingProperties](organizationalbrandingproperties.md) | Obter uma coleção de objetos organizationalBrandingProperties. |

## <a name="properties"></a>Propriedades 
| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| assignedPlans | Coleção [assignedPlan](assignedplan.md) | A coleção de planos de serviço associados ao locatário. Não anulável. |
| businessPhones | Coleção de cadeias de caracteres | Número de telefone da organização. **Observação:** embora essa seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade. |
| city | Cadeia de caracteres | Nome da cidade do endereço da organização. |
| country | Cadeia de caracteres | Nome do país/região do endereço da organização. |
| countryLetterCode | Cadeia de caracteres | Abreviação do país/região da organização. |
| createdDateTime | DateTimeOffset | Carimbo de hora de criação da organização. Não é possível modificar o valor e ele é preenchido automaticamente quando a organização é criada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| deletedDateTime | DateTimeOffset | Representa a data e a hora que o locatário do Azure AD foi excluído usando o formato ISO 8601 e está sempre no horário do UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
| directorySizeQuota | [directorySizeQuota](directorySizeQuota.md) | As informações de cota de tamanho do diretório de uma organização. |
| displayName | String | O nome de exibição do locatário. |
| id | Cadeia de caracteres | A ID do locatário, um identificador exclusivo que representa a organização (ou Locatário). Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. |
| isMultipleDataLocationsForServicesEnabled | Boolean | **verdadeiro** se a organização estiver habilitada no Multi-Geo; **falso** se a organização não estiver habilitada no Multi-Geo, **nulo** (padrão). Somente leitura. Para saber mais, confira [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction). |
| marketingNotificationEmails | Coleção de cadeias de caracteres | Não anulável. |
| objectType | String | Uma cadeia de caracteres que identifica o tipo de objeto. Para locatários, o valor é sempre "Empresa". |
| onPremisesLastSyncDateTime | DateTimeOffset | A hora e a data em que o locatário foi sincronizado pela última vez com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
| onPremisesSyncEnabled | Booliano | **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). |
| postalCode | Cadeia de caracteres | CEP do endereço da organização. |
| preferredLanguage | String | O idioma preferencial da organização. Deve seguir o código ISO 639-1; por exemplo "en". |
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
|certificateBasedAuthConfiguration|coleção [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md)| Propriedade navigation para gerenciar a configuração de autenticação baseada em certificado. Somente uma única instância de certificateBasedAuthConfiguration pode ser criada na coleção.  |
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para o recurso da organização. Anulável.| 
|organizationalBranding|[Coleção organizationalBrandingProperties](organizationalbrandingproperties.md)| Identidade visual para a organização. Anulável.|
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
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
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
