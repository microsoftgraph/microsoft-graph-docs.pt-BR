---
title: Criar intuneBrandingProfile
description: Crie um novo objeto intuneBrandingProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e6b8d89b2575402cc38b5f86ecd8a872fd666b3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133847"
---
# <a name="create-intunebrandingprofile"></a>Criar intuneBrandingProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto intuneBrandingProfile.](../resources/intune-wip-intunebrandingprofile.md)

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
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto intuneBrandingProfile.

A tabela a seguir mostra as propriedades que são necessárias ao criar o intuneBrandingProfile.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave de Perfil|
|profileName|Cadeia de caracteres|Nome do perfil|
|profileDescription|Cadeia de caracteres|Descrição do perfil|
|isDefaultProfile|Booleano|Boolean que representa se o perfil é usado como padrão ou não|
|createdDateTime|DateTimeOffset|Hora em que o BrandingProfile foi criado|
|lastModifiedDateTime|DateTimeOffset|Hora em que o BrandingProfile foi modificado pela última vez|
|displayName|Cadeia de caracteres|Nome da empresa/organização exibido para usuários finais|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor de tema principal usada nos aplicativos do Portal da Empresa e no portal da Web|
|showLogo|Booliano|Boolean que representa se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
|showDisplayNameNextToLogo|Booliano|Boolean que representa se o nome de exibição fornecido pelo administrador será mostrado ao lado da imagem de logotipo ou não|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida em aplicativos do Portal da Empresa que têm um plano de fundo de cor de tema atrás do logotipo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem de logotipo exibida em aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem personalizada exibida na página inicial de aplicativos do Portal da Empresa|
|contactITName|Cadeia de caracteres|Nome da pessoa/organização responsável pelo suporte a IT|
|contactITPhoneNumber|Cadeia de caracteres|Número de telefone da pessoa/organização responsável pelo suporte a IT|
|contactITEmailAddress|Cadeia de caracteres|Endereço de email da pessoa/organização responsável pelo suporte a IT|
|contactITNotes|Cadeia de caracteres|Comentários de texto sobre a pessoa/organização responsável pelo suporte a IT|
|onlineSupportSiteUrl|Cadeia de caracteres|URL para o site de ajuda de IT da empresa/organização|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de ajuda de IT da empresa/organização|
|privacyUrl|Cadeia de caracteres|URL para a política de privacidade da empresa/organização|
|customPrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador não tem acesso no dispositivo|
|customCanSeePrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador tem acesso no dispositivo|
|customCantSeePrivacyMessage|Cadeia de caracteres|Comentários de texto sobre o que o administrador não tem acesso no dispositivo|
|isRemoveDeviceDisabled|Booleano|Boolean que representa se o administrador desabilitou a ação "Remover Dispositivo" em dispositivos de propriedade corporativa.|
|isFactoryResetDisabled|Booleano|Boolean que representa se o administrador desabilitou a ação 'Redefinição de Fábrica' em dispositivos de propriedade corporativa.|
|companyPortalBlockedActions|[Coleção companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Coleção de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade da plataforma e do dispositivo.|
|showAzureADEnterpriseApps|Booleano|Boolean que indica se os aplicativos corporativos do AzureAD serão mostrados no Portal da Empresa|
|showOfficeWebApps|Booleano|Boolean que indica se o Office WebApps será mostrado no Portal da Empresa|
|sendDeviceOwnershipChangePushNotification|Booleano|Boolean que indica se uma notificação por push é enviada aos usuários quando o tipo de propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final . Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|disableClientTelemetry|Booleano|Aplica-se à telemetria enviada de todos os clientes para o serviço do Intune. Quando desabilitado, todos os avisos de solução de problemas e problemas proativos dentro do cliente são desativados, e as configurações de telemetria aparecem inativas ou ocultas para o usuário do dispositivo.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo atribuídas ao perfil de identidade visual|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
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
HTTP/1.1 201 Created
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




