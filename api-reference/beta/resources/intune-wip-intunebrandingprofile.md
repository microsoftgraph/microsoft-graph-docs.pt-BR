---
title: tipo de recurso intuneBrandingProfile
description: Esta entidade contém dados que são usados na personalização da aparência do nível do locatário dos aplicativos do portal da empresa, bem como do portal da Web do usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c47ba76846586ffdf355f433538288267347bc0b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258596"
---
# <a name="intunebrandingprofile-resource-type"></a>tipo de recurso intuneBrandingProfile

Namespace: microsoft.graph

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
|displayName|String|Nome da empresa/organização que é exibido para os usuários finais|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo de cor de tema atrás do logotipo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do portal da empresa que têm um plano de fundo claro atrás do logotipo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial dos aplicativos do portal da empresa|
|contactITName|Cadeia de caracteres|Nome da pessoa/organização responsável pelo suporte de ti|
|contactITPhoneNumber|Cadeia de caracteres|Número de telefone da pessoa/organização responsável pelo suporte de ti|
|contactITEmailAddress|Cadeia de caracteres|Endereço de email da pessoa/organização responsável pelo suporte de ti|
|contactITNotes|Cadeia de caracteres|Comentários de texto sobre a pessoa/organização responsável pelo suporte de ti|
|onlineSupportSiteUrl|Cadeia de caracteres|URL para o site de assistência técnica de ti da empresa/organização|
|onlineSupportSiteName|Cadeia de caracteres|Nome para exibição do site de assistência técnica de ti da empresa/organização|
|privacyUrl|Cadeia de caracteres|URL para a política de privacidade da empresa/organização|
|customPrivacyMessage|String|Comentários de texto sobre o que o administrador não tem acesso ao no dispositivo|
|customCanSeePrivacyMessage|String|Comentários de texto sobre o que o administrador tem acesso ao no dispositivo|
|customCantSeePrivacyMessage|String|Comentários de texto sobre o que o administrador não tem acesso ao no dispositivo|
|isRemoveDeviceDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.|
|isFactoryResetDisabled|Booliano|Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.|
|companyPortalBlockedActions|coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.|
|showAzureADEnterpriseApps|Booliano|Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa|
|showOfficeWebApps|Booliano|Booliano que indica se o Office webapps será mostrado no portal da empresa|
|sendDeviceOwnershipChangePushNotification|Booliano|Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final. Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|disableClientTelemetry|Booliano|Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune. Quando desabilitado, todos os avisos proativos de solução de problemas e emissão dentro do cliente estão desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.|
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




