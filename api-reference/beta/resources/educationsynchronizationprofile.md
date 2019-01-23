---
title: tipo de recurso de educationSynchronizationProfile
description: Representa um conjunto de configurações usadas para sincronizar as informações de lista de participação de um diretório de origem para o Windows Azure Active Directory (AD Azure) e entidades de educação. Esse recurso fornece uma representação programática usada na sincronização de dados da escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b753e904a0c70d5c0ae83dbb3d9a88aff8401eac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396949"
---
# <a name="educationsynchronizationprofile-resource-type"></a>tipo de recurso de educationSynchronizationProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um conjunto de configurações usadas para sincronizar as informações de lista de participação de um diretório de origem para o Windows Azure Active Directory (AD Azure) e entidades de educação. Esse recurso fornece uma representação programática usada na [Sincronização de dados da escola](https://sds.microsoft.com).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Perfis de sincronização de lista](../api/educationsynchronizationprofile-list.md) | coleção **educationSynchronizationProfile** | Obtenha uma lista de todos os perfis de sincronização no inquilino. |
| [Obtenha o perfil de sincronização](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | Recupere um perfil específico, dado o identificador do perfil. |
| [Criar um perfil de sincronização](../api/educationsynchronizationprofile-post.md) | Nenhum | Crie um novo perfil de sincronização. |
| [Excluir o perfil de sincronização](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | Exclua um perfil específico, dado o identificador do perfil. |
| [Pausar uma sincronização em andamento](../api/educationsynchronizationprofile-pause.md) | Nenhum | Pause uma sincronização em andamento. |
| [Retomar uma sincronização pausada](../api/educationsynchronizationprofile-resume.md) | Nenhum | Retome uma sincronização pausada. |
| [Redefinir uma sincronização](../api/educationsynchronizationprofile-reset.md) | Nenhum | Redefinir o estado do perfil e reinicie a sincronização. |
| [Iniciar sincronização para arquivos carregados](../api/educationsynchronizationprofile-start.md) | coleção [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md)| Verifique se os arquivos de origem carregado e iniciar a sincronização. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Obtenha uma URL de carregamento](../api/educationsynchronizationprofile-uploadurl.md) | string | Retorne a URL temporários e para carregar arquivos de dados CSV. Aplica-se somente quando o provedor de dados é [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Obter o status de uma sincronização](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Retorna o status de um perfil de sincronização específico. |
| [Obtenha os erros de sincronização](../api/educationsynchronizationerrors-get.md) | coleção [educationSynchronizationError](educationsynchronizationerror.md)| Obtenha todos os erros gerados durante a sincronização. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **displayName** | string |  Nome do perfil de configuração para sincronização de identidades.         |
| **dataProvider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  O provedor de dados usado para o perfil.         |
| **identitySynchronizationConfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | Configuração de [criação](educationidentitycreationconfiguration.md) ou [correspondentes](educationidentitymatchingconfiguration.md) da identidade.        |
| **licensesToAssign** | coleção [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md)|  Configuração de licença.        |
| **state** | educationSynchronizationProfileState |  O estado do perfil. Os valores possíveis são: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.          |

## <a name="relationships"></a>Relações

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **errors** | coleção [educationSynchronizationError](educationsynchronizationerror.md)| Todos os erros associados a esse perfil de sincronização. |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | O status da sincronização. |

## <a name="json-representation"></a>Representação JSON
A seguir está uma representação JSON do recurso **educationSynchronizationProfile** .

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
