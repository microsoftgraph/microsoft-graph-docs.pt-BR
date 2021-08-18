---
title: Tipo de recurso intuneBrandingProfile
description: Essa entidade contém dados usados para personalizar a aparência de nível de locatário dos aplicativos Portal da Empresa, bem como o portal da Web do usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 15fbf2802b078214c0c78e11576364ee074560645f471122d56bda2cccfc7dc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209774"
---
# <a name="intunebrandingprofile-resource-type"></a>Tipo de recurso intuneBrandingProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade contém dados usados para personalizar a aparência de nível de locatário dos aplicativos Portal da Empresa, bem como o portal da Web do usuário final.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[Coleção intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Listar propriedades e relações dos objetos [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Obter intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Ler propriedades e relações do objeto [intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Criar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Crie um novo [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[Excluir intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|Nenhum|Exclui um [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Atualizar intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Atualize as propriedades de um [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)|
|[atribuir ação](../api/intune-wip-intunebrandingprofile-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave de Perfil|
|profileName|Cadeia de caracteres|Nome do perfil|
|profileDescription|Cadeia de caracteres|Descrição do perfil|
|isDefaultProfile|Boolean|Boolean que representa se o perfil é usado como padrão ou não|
|createdDateTime|DateTimeOffset|Hora em que o BrandingProfile foi criado|
|lastModifiedDateTime|DateTimeOffset|Hora em que o BrandingProfile foi modificado pela última vez|
|displayName|Cadeia de caracteres|Nome da empresa/organização exibido para usuários finais|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor de tema principal usada nos aplicativos Portal da Empresa web e portal da Web|
|showLogo|Booliano|Boolean que representa se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
|showDisplayNameNextToLogo|Booliano|Boolean que representa se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida em Portal da Empresa que têm um plano de fundo de cor de tema atrás do logotipo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida em Portal da Empresa que têm um plano de fundo claro atrás do logotipo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial Portal da Empresa aplicativos|
|contactITName|Cadeia de caracteres|Nome da pessoa/organização responsável pelo suporte a IT|
|contactITPhoneNumber|Cadeia de caracteres|Telefone número da pessoa/organização responsável pelo suporte a IT|
|contactITEmailAddress|Cadeia de caracteres|Endereço de email da pessoa/organização responsável pelo suporte a IT|
|contactITNotes|Cadeia de caracteres|Comentários de texto sobre a pessoa/organização responsável pelo suporte a IT|
|onlineSupportSiteUrl|Cadeia de caracteres|URL para o site de ajuda de IT da empresa/organização|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de ajuda de IT da empresa/organização|
|privacyUrl|Cadeia de caracteres|URL para a política de privacidade da empresa/organização|
|customPrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador não tem acesso no dispositivo|
|customCanSeePrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador tem acesso no dispositivo|
|customCantSeePrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador não tem acesso no dispositivo|
|isRemoveDeviceDisabled|Boolean|Boolean que representa se o administrador desabilitou a ação "Remover Dispositivo" em dispositivos de propriedade corporativa.|
|isFactoryResetDisabled|Boolean|Boolean que representa se o administrador desabilitou a ação 'Redefinição de Fábrica' em dispositivos de propriedade corporativa.|
|companyPortalBlockedActions|[Coleção companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Coleção de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade da plataforma e do dispositivo.|
|showAzureADEnterpriseApps|Boolean|Boolean que indica se os aplicativos Enterprise AzureAD serão mostrados em Portal da Empresa|
|showOfficeWebApps|Boolean|Boolean que indica se Office WebApps serão mostrados em Portal da Empresa|
|sendDeviceOwnershipChangePushNotification|Boolean|Boolean que indica se uma notificação por push é enviada aos usuários quando o tipo de propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final . Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|disableClientTelemetry|Boolean|Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune. Quando desabilitado, todos os avisos de solução de problemas e problemas proativos dentro do cliente são desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.|
|roleScopeTagIds|String collection|Lista de marcas de escopo atribuídas ao perfil de identidade visual|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)|A lista de atribuições de grupo para o perfil de identidade visual|

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
  "customCanSeePrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
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
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




