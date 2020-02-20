---
title: tipo de recurso intuneBrandingProfile
description: Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f161b0354e9fd2a4e8cf7a5e5936d2cf2719a407
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163700"
---
# <a name="intunebrandingprofile-resource-type"></a>tipo de recurso intuneBrandingProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar Navegaçãointunebrandingprofiles](../api/intune-wip-intunebrandingprofile-list.md)|coleção [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Listar Propriedades e relações dos objetos [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Obter intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Leia as propriedades e as relações do objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Criar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[Excluir intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Nenhum|Exclui [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Atualizar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Atualiza as propriedades de um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .|
|[atribuir ação](../api/intune-wip-intunebrandingprofile-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|ProfileName|String|Nome do perfil|
|profileDescription|String|Descrição do perfil|
|isDefaultProfile|Booliano|Booliano que indica se o perfil é usado como padrão ou não|
|createdDateTime|DateTimeOffset|Hora em que o BrandingProfile foi criado|
|lastModifiedDateTime|DateTimeOffset|Hora em que a BrandingProfile foi modificada pela última vez|
|displayName|Cadeia de caracteres|Nome da empresa/organização que é exibido para os usuários finais|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa|
|contactITName|String|Nome da pessoa/organização responsável pelo suporte de ti|
|contactITPhoneNumber|String|Número de telefone da pessoa/organização responsável pelo suporte de ti|
|contactITEmailAddress|String|Endereço de email da pessoa/organização responsável pelo suporte de ti|
|contactITNotes|String|Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti|
|onlineSupportSiteUrl|String|URL para o site de assistência técnica de ti da empresa/organização|
|onlineSupportSiteName|Cadeia de caracteres|Nome para exibição do site de assistência técnica de ti da empresa/organização|
|privacyUrl|String|URL para a política de privacidade da empresa/organização|
|customPrivacyMessage|String|Comentários de texto sobre o que o administrador tem acesso ao no dispositivo|
|isRemoveDeviceDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.|
|isFactoryResetDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.|
|companyPortalBlockedActions|coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.|
|showAzureADEnterpriseApps|Booliano|Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa|
|showOfficeWebApps|Booliano|Booliano que indica se o Office webapps será mostrado no portal da empresa|
|sendDeviceOwnershipChangePushNotification|Booliano|Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final. Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo atribuídas ao perfil de identidade visual|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|A lista de atribuições de grupo para o perfil de identidade visual|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```



