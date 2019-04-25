---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e1b81ff14aca2b0f81a7f50e01aed6281d03d14d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542864"
---
# <a name="educationsynchronizationprofile-resource-type"></a>tipo de recurso educationSynchronizationProfile

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Listar perfis de sincronização](../api/educationsynchronizationprofile-list.md) | coleção **educationSynchronizationProfile** | Obtenha uma lista de todos os perfis de sincronização no locatário. |
| [Obter perfil de sincronização](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | Recupere um perfil específico dado o identificador de perfil. |
| [Criar perfil de sincronização](../api/educationsynchronizationprofile-post.md) | Nenhum | Criar um novo perfil de sincronização. |
| [Excluir perfil de sincronização](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | Excluir um perfil específico dado o identificador de perfil. |
| [PaUsar uma sincronização contínua](../api/educationsynchronizationprofile-pause.md) | Nenhum | PaUsar uma sincronização em andamento. |
| [ReTomar uma sincronização pausada](../api/educationsynchronizationprofile-resume.md) | Nenhum | ReTomar uma sincronização pausada. |
| [Redefinir uma sincronização](../api/educationsynchronizationprofile-reset.md) | Nenhum | ReDefina o estado do perfil e reinicie a sincronização. |
| [Iniciar a sincronização de arquivos carregados](../api/educationsynchronizationprofile-start.md) | coleção [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)| Verifique os arquivos de origem carregados e inicie a sincronização. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Obter uma URL de upload](../api/educationsynchronizationprofile-uploadurl.md) | string | Retornar a URL de curta duração para carregar arquivos de dados CSV. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Retornar o status de um perfil de sincronização específico. |
| [Obter erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção [educationSynchronizationError](educationsynchronizationerror.md)| Obtenha todos os erros gerados durante a sincronização. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **displayName** | string |  Nome do perfil de configuração para sincronizar identidades.         |
| **DataProvider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  O provedor de dados usado para o perfil.         |
| **identitySynchronizationConfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | [Criação](educationidentitycreationconfiguration.md) de identidade ou configuração de [correspondência](educationidentitymatchingconfiguration.md) .        |
| **licensesToAssign** | coleção [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)|  Configuração da instalação da licença.        |
| **state** | educationSynchronizationProfileState |  O estado do perfil. Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.          |

## <a name="relationships"></a>Relações

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **errors** | coleção [educationSynchronizationError](educationsynchronizationerror.md)| Todos os erros associados a este perfil de sincronização. |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | O status da sincronização. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso **educationSynchronizationProfile** .

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
