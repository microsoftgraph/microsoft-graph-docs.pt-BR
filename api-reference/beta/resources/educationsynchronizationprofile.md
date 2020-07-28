---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86c8189e170bba5899f82f75902dfe68dd0d3fd1
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434906"
---
# <a name="educationsynchronizationprofile-resource-type"></a>tipo de recurso educationSynchronizationProfile

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Métodos

| Método                                                                    | Tipo de retorno                                                 | Descrição                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [Listar perfis](../api/educationsynchronizationprofile-list.md)           | coleção [educationSynchronizationProfile]                | Obtenha uma lista de todos os perfis de sincronização no locatário.                                                                  |
| [Obter perfil](../api/educationsynchronizationprofile-get.md)              | [educationSynchronizationProfile]                           | Recupere um perfil específico dado o identificador de perfil.                                                                      |
| [Criar perfil](../api/educationsynchronizationprofile-post.md)          | Nenhum                                                        | Criar um novo perfil de sincronização.                                                                                          |
| [Excluir perfil](../api/educationsynchronizationprofile-delete.md)        | [educationSynchronizationProfile]                           | Excluir um perfil específico dado o identificador de perfil.                                                                        |
| [Pausar perfil](../api/educationsynchronizationprofile-pause.md)          | Nenhum                                                        | Pausar uma sincronização em andamento.                                                                                              |
| [Retomar perfil](../api/educationsynchronizationprofile-resume.md)        | Nenhum                                                        | Retomar uma sincronização pausada.                                                                                               |
| [Redefinir perfil](../api/educationsynchronizationprofile-reset.md)          | Nenhum                                                        | Redefina o estado do perfil e reinicie a sincronização.                                                                    |
| [Iniciar perfil CSV](../api/educationsynchronizationprofile-start.md)      | coleção [educationFileSynchronizationVerificationMessage] | Verifique os arquivos de origem carregados e inicie a sincronização. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider]. |
| [Obter URL de upload de CSV](../api/educationsynchronizationprofile-uploadurl.md) | cadeia de caracteres                                                      | Retornar a URL de curta duração para carregar arquivos de dados CSV. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider].        |
| [Obter status](../api/educationsynchronizationprofilestatus-get.md)         | [educationsynchronizationProfileStatus]                     | Retornar o status de um perfil de sincronização específico.                                                                       |
| [Obter erros](../api/educationsynchronizationerrors-get.md)                | coleção [educationSynchronizationError]                  | Obtenha todos os erros gerados durante a sincronização.                                                                           |

## <a name="properties"></a>Propriedades

| Propriedade                             | Tipo                                                   | Descrição                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| id                                   | String                                                 | O identificador exclusivo do recurso. (somente leitura)                                                                               |
| displayName                          | Cadeia de caracteres                                                 | Nome do perfil de configuração para sincronizar identidades.                                                                         |
| DataProvider                         | [educationSynchronizationDataProvider]                 | O provedor de dados usado para o perfil.                                                                                           |
| expirationDate                       | Data                                                   | A data em que o perfil deve ser considerado expirado e parar a sincronização. Quando `null` . o perfil nunca expirará. (opcional)       |
| handleSpecialCharacterConstraint     | Bool                                                   | Determina se a escola de sincronização de dados deve substituir automaticamente caracteres especiais não suportados durante a sincronização da origem.             |
| identitySynchronizationConfiguration | [educationIdentitySynchronizationConfiguration]        | Determina como o perfil deve [criar usuários novos][fullsync] ou [correspondentes existentes][dirsync] do AAD.                                  |
| licensesToAssign                     | coleção [educationSynchronizationLicenseAssignment] | Configuração da instalação da licença.                                                                                                      |
| state                                | educationSynchronizationProfileState                   | O estado do perfil. Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`. |

## <a name="relationships"></a>Relações

| Relação  | Tipo                                       | Descrição                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| erros        | coleção [educationSynchronizationError] | Todos os erros associados a este perfil de sincronização. |
| profileStatus | [educationSynchronizationProfileStatus]    | O status da sincronização.                              |

## <a name="data-providers"></a>Provedores de dados

Cada [educationSynchronizationProfile] deve especificar um dos provedores de dados a seguir para usar como a fonte de sincronização.

| Data Provider                                                             | Descrição                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | API do OneRoster v 1.1                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API da PowerSchool                                                                                    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso **educationSynchronizationProfile** .

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
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
