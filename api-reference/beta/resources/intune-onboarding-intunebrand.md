---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a30454de5ab8ccbe577c10ceddbe887a0f10a9eb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816447"
---
# <a name="intunebrand-resource-type"></a>Tipo de recurso intuneBrand

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome da empresa/organização exibido para usuários finais.|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.|
|showLogo|Booliano|Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.|
|showNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial Portal da Empresa aplicativo|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo atribuídas ao perfil de identidade visual padrão|
|contactITName|Cadeia de caracteres|Nome da pessoa/organização responsável pelo suporte de TI.|
|contactITPhoneNumber|Cadeia de caracteres|Número de telefone da pessoa/organização responsável pelo suporte de TI.|
|contactITEmailAddress|Cadeia de caracteres|Endereço de email da pessoa/organização responsável pelo suporte de TI.|
|contactITNotes|Cadeia de caracteres|Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.|
|onlineSupportSiteUrl|Cadeia de caracteres|URL do site de assistência técnica de TI da empresa/organização.|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de assistência técnica de TI da empresa/organização.|
|privacyUrl|Cadeia de caracteres|URL da política de privacidade da empresa/organização.|
|customPrivacyMessage|Cadeia de caracteres|A mensagem de privacidade personalizada usada para explicar o que a organização não pode ver ou fazer em dispositivos gerenciados.|
|customCantSeePrivacyMessage|Cadeia de caracteres|A mensagem de privacidade personalizada usada para explicar o que a organização não pode ver ou fazer em dispositivos gerenciados.|
|customCanSeePrivacyMessage|Cadeia de caracteres|A mensagem de privacidade personalizada usada para explicar o que a organização pode ver e fazer em dispositivos gerenciados.|
|isRemoveDeviceDisabled|Booliano|Boolean que representa se o administrador desabilitou a ação "Remover Dispositivo" em dispositivos de propriedade corporativa.|
|isFactoryResetDisabled|Boolean|Boolean que representa se o administrador desabilitou a ação 'Redefinição de Fábrica' em dispositivos de propriedade corporativa.|
|companyPortalBlockedActions|[Coleção companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Coleção de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade da plataforma e do dispositivo.|
|showAzureADEnterpriseApps|Booliano|Boolean que indica se os aplicativos Enterprise AzureAD serão mostrados em Portal da Empresa|
|showOfficeWebApps|Boolean|Boolean que indica se Office WebApps serão mostrados em Portal da Empresa|
|sendDeviceOwnershipChangePushNotification|Booliano|Boolean que indica se uma notificação por push é enviada aos usuários quando o tipo de propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final . Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|disableClientTelemetry|Booliano|Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune. Quando desabilitado, todos os avisos de solução de problemas e problemas proativos dentro do cliente são desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
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
  "disableClientTelemetry": true
}
```



