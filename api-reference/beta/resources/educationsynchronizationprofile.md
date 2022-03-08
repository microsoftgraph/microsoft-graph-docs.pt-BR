---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para Azure Active Directory (Azure AD). Esse recurso fornece uma representação programática usada em School Data Sync.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e3b687e3856ae8d7805bf4b74724c70380359a9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336001"
---
# <a name="educationsynchronizationprofile-resource-type"></a>tipo de recurso educationSynchronizationProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para Azure Active Directory (Azure AD). Esse recurso fornece uma representação programática usada em [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Métodos

| Método                                                                    | Tipo de retorno                                                 | Descrição                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [Listar perfis](../api/educationsynchronizationprofile-list.md)           | [coleção educationSynchronizationProfile]                | Obter uma lista de todos os perfis de sincronização no locatário.                                                                  |
| [Obter perfil](../api/educationsynchronizationprofile-get.md)              | [educationSynchronizationProfile]                           | Recupere um perfil específico, dado o identificador de perfil.                                                                      |
| [Criar perfil](../api/educationsynchronizationprofile-post.md)          | Nenhum                                                        | Crie um novo perfil de sincronização.                                                                                          |
| [Excluir perfil](../api/educationsynchronizationprofile-delete.md)        | [educationSynchronizationProfile]                           | Exclua um perfil específico dado o identificador de perfil.                                                                        |
| [Pausar perfil](../api/educationsynchronizationprofile-pause.md)          | Nenhum                                                        | Pause uma sincronização contínua.                                                                                              |
| [Retomar perfil](../api/educationsynchronizationprofile-resume.md)        | Nenhum                                                        | Retomar uma sincronização pausada.                                                                                               |
| [Redefinir perfil](../api/educationsynchronizationprofile-reset.md)          | Nenhum                                                        | Redefina o estado do perfil e reinicie a sincronização.                                                                    |
| [Iniciar perfil CSV](../api/educationsynchronizationprofile-start.md)      | [educationFileSynchronizationVerificationMessagecollection] | Verifique os arquivos de origem carregados e inicie a sincronização. Aplica-se somente quando o provedor de dados [é educationCsvDataProvider]. |
| [Obter URL de carregamento CSV](../api/educationsynchronizationprofile-uploadurl.md) | string                                                      | Retorne a URL de curta duração para carregar arquivos de dados CSV. Aplica-se somente quando o provedor de dados [é educationCsvDataProvider].        |
| [Obter status](../api/educationsynchronizationprofilestatus-get.md)         | [educationsynchronizationProfileStatus]                     | Retorne o status de um perfil de sincronização específico.                                                                       |
| [Obter erros](../api/educationsynchronizationerrors-get.md)                | [coleção educationSynchronizationError]                  | Obter todos os erros gerados durante a sincronização.                                                                           |

## <a name="properties"></a>Propriedades

| Propriedade                             | Tipo                                                   | Descrição                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| id                                   | String                                                 | O identificador exclusivo do recurso. (somente leitura)                                                                               |
| displayName                          | String                                                 | Nome do perfil de configuração para sincronização de identidades.                                                                         |
| dataProvider                         | [educationSynchronizationDataProvider]                 | O provedor de dados usado para o perfil.                                                                                           |
| expirationDate                       | Data                                                   | A data em que o perfil deve ser considerado expirado e interromper a sincronização. Forneça a data em formato `YYYY-MM-DD` , seguindo [a ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). O valor máximo é 18 meses após a criação do perfil.  (opcional)       |
| handleSpecialCharacterConstraint     | Bool                                                   | Determina se o School Data Sync deve substituir automaticamente caracteres especiais sem suporte durante a sincronização da origem.             |
| identitySynchronizationConfiguration | [educationIdentitySynchronizationConfiguration]        | Determina como o Perfil deve [criar novos ou][fullsync] [corresponder aos][dirsync] usuários AAD existentes.                                  |
| licensesToAssign                     | [coleção educationSynchronizationLicenseAssignment] | Configuração de configuração de licença.                                                                                                      |
| state                                | educationSynchronizationProfileState                   | O estado do perfil. Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`. |

## <a name="relationships"></a>Relações

| Relação  | Tipo                                       | Descrição                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| erros        | [coleção educationSynchronizationError] | Todos os erros associados a esse perfil de sincronização. |
| profileStatus | [educationSynchronizationProfileStatus]    | O status de sincronização.                              |

## <a name="data-providers"></a>Provedores de dados

Cada [educationSynchronizationProfile] deve especificar um dos provedores de dados a seguir a ser usado como fonte de sincronização.

| Data Provider                                                             | Descrição                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | Arquivos CSV carregados na [URL SAS do Perfil](../api/educationsynchronizationprofile-uploadurl.md) |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API da PowerSchool                                                                                    |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do **recurso educationSynchronizationProfile** .

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
}-->


