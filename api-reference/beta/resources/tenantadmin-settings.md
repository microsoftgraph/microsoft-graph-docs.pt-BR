---
title: tipo de recurso de configurações
description: Representa as configurações no nível do locatário para SharePoint e OneDrive.
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: acc37088c339abeaf0e6405e00ef45a344803e9c
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653597"
---
# <a name="settings-resource-type"></a>tipo de recurso de configurações
Namespace: microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações no nível do locatário para SharePoint e OneDrive.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição
|:---|:---|:---
|[Obter configurações](../api/tenantadmin-settings-get.md)|[microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | Obtenha as configurações no nível do locatário para SharePoint e OneDrive.|
|[Atualizar configurações](../api/tenantadmin-settings-update.md) | [microsoft.graph.tenantAdmin.settings](../resources/tenantadmin-settings.md) | Atualize uma ou mais configurações de nível de locatário SharePoint e OneDrive.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | Coleção de GUIDs              | Coleção de GUIDs de domínio confiável para o Sincronização do OneDrive aplicativo.                                                                                                                                                  |
| availableManagedPathsForSiteCreation               | Coleção de cadeias de caracteres            | Coleção de caminhos gerenciados disponíveis para a criação do site. Somente leitura.                                                                                                                                            |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | O número de dias para preservar os dados de um usuário excluído OneDrive.                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | Coleção de cadeias de caracteres            | Coleção de extensões de arquivo não carregadas pelo Sincronização do OneDrive aplicativo.                                                                                                                                           |
| imageTaggingOption                                 | [tenantAdmin.imageTaggingChoice](../resources/tenantadmin-settings.md#imagetaggingchoice-values)           | Especifica a opção de marcação de imagem para o locatário. Os valores possíveis são: `disabled`, `basic`, `enhanced`.                                                                                                       |
| isCommentingOnSitePagesEnabled                     | Booliano                      | Indica se os comentários são permitidos em páginas de site modernas SharePoint.                                                                                                                                          |
| isFileActivityNotificationEnabled                  | Boolean                      | Indica se as notificações por push estão habilitadas para OneDrive eventos.                                                                                                                                               |
| isLoopEnabled                                      | Booliano                      | Indica se a Fluid Framework é permitida em SharePoint sites.                                                                                                                                                   |
| isMacSyncAppEnabled                                | Boolean                      | Indica se os arquivos podem ser sincronizados usando o aplicativo Sincronização do OneDrive para Mac.                                                                                                                                          |
| isResharingByExternalUsersEnabled                  | Booliano                      | Indica se os convidados têm permissão para compartilhar novamente arquivos, pastas e sites que eles não têm.                                                                                                                           |
| isSharePointMobileNotificationEnabled              | Boolean                      | Indica se as notificações por push móveis estão habilitadas para SharePoint.                                                                                                                                             |
| isSharePointNewsfeedEnabled                        | Booliano                      | Indica se o news feed é permitido nas páginas modernas do site SharePoint.                                                                                                                                   |
| isSiteCreationEnabled                              | Boolean                      | Indica se os usuários têm permissão para criar sites.                                                                                                                                                           |
| isSiteCreationUIEnabled                            | Booliano                      | Indica se os comandos da interface do usuário para criar sites são mostrados.                                                                                                                                                     |
| isSitePagesCreationEnabled                         | Boolean                      | Indica se a criação de novas páginas modernas é permitida SharePoint sites.                                                                                                                                         |
| isSitesStorageLimitAutomatic                       | Booliano                      | Indica se o espaço de armazenamento do site é gerenciado automaticamente ou se os limites de armazenamento específicos são definidos por site.                                                                                                       |
| isSyncButtonHiddenOnPersonalSite                   | Boolean                      | Indica se o botão de sincronização no OneDrive está oculto.                                                                                                                                                            |
| isUnmanagedSyncAppForTenantRestricted              | Booliano                      | Indica se os usuários têm permissão para sincronizar arquivos somente em computadores ingressados em domínios específicos.                                                                                                                           |
| personalSiteDefaultStorageLimitInMB                | Int64                        | O padrão OneDrive limite de armazenamento para todos os usuários novos e existentes que recebem uma licença qualificada. Medido em megabytes (MB).                                                                           |
| sharingAllowedDomainList                           | Coleção de cadeias de caracteres            | Coleção de domínios de email permitidos para compartilhamento fora da organização.                                                                                                                              |
| sharingBlockedDomainList                           | Coleção de cadeias de caracteres            | Coleção de domínios de email bloqueados para compartilhamento fora da organização.                                                                                                                              |
| sharingCapability                                  | [tenantAdmin.sharingCapabilities](#sharingcapabilities-values)          | Capacidade de compartilhamento para o locatário. Os valores possíveis são: `disabled`, `externalUserSharingOnly`, `externalUserAndGuestSharing`, `existingExternalUserSharingOnly`.                                                |
| sharingDomainRestrictionMode                       | [tenantAdmin.sharingDomainRestrictionMode](#sharingdomainrestrictionmode-values) | Especifica o modo compartilhamento externo para os domínios. Os valores possíveis são: `none`, `allowList`, `blockList`.                                                                                                        |
| siteCreationDefaultManagedPath                     | Cadeia de caracteres                       | O valor do caminho gerenciado do site de equipe. Esse é o caminho no qual novos sites de equipe serão criados.                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | A cota de armazenamento padrão para um novo site após a criação. Medido em megabytes (MB).                                                                                                                            |
| tenantDefaultTimezone                              | Cadeia de caracteres                       | O fuso horário padrão de um locatário para sites recém-criados.                                                                                                                                                      |

### <a name="imagetaggingchoice-values"></a>Valores imageTaggingChoice
| Member                          | Descrição                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| desabilitadas                        | A opção de marcação de imagem para o locatário está desabilitada.                                                                  |
| Basic                           | Permite que os usuários dentro do locatário adicionem marcas básicas a imagens para torná-las acessíveis por meio da pesquisa.                    |
| Reforçada                        | Permite que os usuários marquem imagens com marcas personalizadas e recursos aprimorados.                                                    |
| unknownFutureValue              | Valor de sentinel de enumeração evolvável. Não usar.                                                                     |

### <a name="sharingcapabilities-values"></a>Valores sharingCapabilities
| Member                          | Descrição                                                                                                           |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------|
| desabilitadas                        | Os usuários só podem compartilhar com pessoas na organização. Nenhum compartilhamento externo é permitido.                                 |
| externalUserSharingOnly         | Os usuários podem compartilhar com convidados novos e existentes. Os convidados devem entrar ou fornecer um código de verificação.                     |
| externalUserAndGuestSharing     | Os usuários podem compartilhar com qualquer pessoa usando links que não exigem entrada.                                                |
| existingExternalUserSharingOnly | Os usuários podem compartilhar com convidados existentes (aqueles que já estão no diretório da organização).                            |
| unknownFutureValue              | Valor de sentinel de enumeração evolvável. Não usar.                                                                     |

### <a name="sharingdomainrestrictionmode-values"></a>Valores sharingDomainRestrictionMode
| Member                          | Descrição                                                                                                           |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| none                            | Nenhuma restrição se aplica.                                                                                                |
| allowList                       | Os usuários poderão compartilhar com colaboradores externos provenientes apenas da lista de domínios de email permitidos.           |
| Blocklist                       | Os usuários poderão compartilhar com todos os colaboradores externos, exceto aqueles na lista de domínios de email bloqueados. |
| unknownFutureValue              | Valor de sentinel de enumeração evolvável. Não usar.                                                                     |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tenantAdmin.settings",
  "openType": "false"
}
-->
``` json
{
    "allowedDomainGuidsForSyncApp": ["string (identifier)"],
    "availableManagedPathsForSiteCreation": ["string"],
    "deletedUserPersonalSiteRetentionPeriodInDays": "Int32",
    "excludedFileExtensionsForSyncApp": ["string"],
    "id": "string (identifier)",
    "imageTaggingOption": "string",
    "isCommentingOnSitePagesEnabled": "boolean",
    "isFileActivityNotificationEnabled": "boolean",
    "isLoopEnabled": "boolean",
    "isMacSyncAppEnabled": "boolean",
    "isResharingByExternalUsersEnabled": "boolean",
    "isSharePointMobileNotificationEnabled": "boolean",
    "isSharePointNewsfeedEnabled": "boolean",
    "isSiteCreationEnabled": "boolean",
    "isSiteCreationUIEnabled": "boolean",
    "isSitePagesCreationEnabled": "boolean",
    "isSitesStorageLimitAutomatic": "boolean",
    "isSyncButtonHiddenOnPersonalSite": "boolean",
    "isUnmanagedSyncAppForTenantRestricted": "boolean",
    "personalSiteDefaultStorageLimitInMB": "Int64",
    "sharingAllowedDomainList" : ["string"],
    "sharingBlockedDomainList" : ["string"],
    "sharingCapability": "string",
    "sharingDomainRestrictionMode": "string",
    "siteCreationDefaultManagedPath": "string",
    "siteCreationDefaultStorageLimitInMB": "Int32",
    "tenantDefaultTimezone": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "namespace": "microsoft.graph.tenantAdmin"
}
-->
