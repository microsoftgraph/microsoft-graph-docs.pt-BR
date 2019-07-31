---
title: tipo de recurso educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar entidades de educação e informações de lista de um diretório de origem para o Azure Active Directory (Azure AD). Este recurso fornece uma representação programática usada no School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5d79c50d29d4a89aa78b724f7cde747ea90706b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972352"
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
| [Pausar uma sincronização contínua](../api/educationsynchronizationprofile-pause.md) | Nenhum | Pausar uma sincronização em andamento. |
| [Retomar uma sincronização pausada](../api/educationsynchronizationprofile-resume.md) | Nenhum | Retomar uma sincronização pausada. |
| [Redefinir uma sincronização](../api/educationsynchronizationprofile-reset.md) | Nenhum | Redefina o estado do perfil e reinicie a sincronização. |
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
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
