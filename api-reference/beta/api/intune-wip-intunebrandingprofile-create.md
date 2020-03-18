---
title: Criar intuneBrandingProfile
description: Criar um novo objeto intuneBrandingProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e67b58af13ec67d157a44b657e019a0bd4c37204
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799735"
---
# <a name="create-intunebrandingprofile"></a>Criar intuneBrandingProfile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementApps.ReadWrite.All|

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
No corpo da solicitação, forneça uma representação JSON do objeto intuneBrandingProfile.

A tabela a seguir mostra as propriedades que são necessárias ao criar intuneBrandingProfile.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave de perfil|
|ProfileName|String|Nome do perfil|
|profileDescription|String|Descrição do perfil|
|isDefaultProfile|Boolean|Booliano que indica se o perfil é usado como padrão ou não|
|createdDateTime|DateTimeOffset|Hora em que o BrandingProfile foi criado|
|lastModifiedDateTime|DateTimeOffset|Hora em que a BrandingProfile foi modificada pela última vez|
|displayName|Cadeia de caracteres|Nome da empresa/organização que é exibido para os usuários finais|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Cor do tema principal usada nos aplicativos do portal da empresa e no portal da Web|
|showLogo|Boolean|Booliano que indica se as imagens de logotipo fornecidas pelo administrador são mostradas ou não|
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
|isRemoveDeviceDisabled|Boolean|Booliano que indica se o adminsistrator desabilitou a ação "remover dispositivo" em dispositivos corporativos de propriedade.|
|isFactoryResetDisabled|Boolean|Booliano que indica se o adminsistrator desabilitou a ação "redefinição de fábrica" em dispositivos corporativos de propriedade.|
|companyPortalBlockedActions|coleção [companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)|Conjunto de ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo.|
|showAzureADEnterpriseApps|Boolean|Booliano que indica se os aplicativos empresariais do AzureAD serão mostrados no portal da empresa|
|showOfficeWebApps|Boolean|Booliano que indica se o Office webapps será mostrado no portal da empresa|
|sendDeviceOwnershipChangePushNotification|Boolean|Booliano que indica se uma notificação por push é enviada aos usuários quando o tipo de Propriedade do dispositivo muda de pessoal para corporativo|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|Fluxo de registro de dispositivo personalizado exibido para o usuário final. Os valores possíveis são: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo atribuídas ao perfil de identidade visual|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1792

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
Content-Length: 1964

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
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




