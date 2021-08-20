---
title: Atualizar intuneBrandingProfile
description: Atualize as propriedades de um objeto intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a066bcb055101b639833f1f81ecca61d57b6acbd716631db67389c7453b5996d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54207240"
---
# <a name="update-intunebrandingprofile"></a>Atualizar intuneBrandingProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).

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



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1975

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2147

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




