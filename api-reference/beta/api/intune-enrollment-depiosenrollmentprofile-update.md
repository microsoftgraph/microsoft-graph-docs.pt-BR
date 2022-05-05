---
title: Atualizar depIOSEnrollmentProfile
description: Atualize as propriedades de um objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a19dbe9fc3e4cb669fb729804006f0d07a14e3f4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209230"
---
# <a name="update-depiosenrollmentprofile"></a>Atualizar depIOSEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [o depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|descrição|Cadeia de caracteres|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de Caracteres|URL do ponto de extremidade de configuração a ser usada para Registro Herdado do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booliano|Indica a autenticação com o Assistente de Configuração da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indica que o Portal da Empresa é necessário em dispositivos registrados do assistente de configuração Herdados do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar; caso contrário, false. Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Cadeia de Caracteres|Informações do departamento de suporte [herdadas de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Booliano|Indica se o perfil é obrigatório Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|Indica se o painel de configuração do serviço local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Cadeia de Caracteres|Suporte ao número de telefone [Herdado de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Booliano|Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|Indica se o painel de instalação restaurar está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Booliano|Indica se o painel de instalação da ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Booliano|Indica se o painel de configuração da ID de toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Booliano|Indica se o painel de instalação da siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnóstico está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Booliano|Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Booliano|Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Booliano|Indica se a configuração de tempo limite da tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Cadeia de Caracteres|Define um literal ou padrão de nome. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Booliano|URL para logon do assistente de configuração Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica o modo de emparelhamento do iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para o Apple Configurator|
|restoreFromAndroidDisabled|Booliano|Indica se a restauração do Android está desabilitada|
|awaitDeviceConfiguredConfirmation|Booliano|Indica se o dispositivo precisará aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Isso especifica o número máximo de usuários que podem usar uma conta iPad. Aplicável somente no modo iPad compartilhado.|
|enableSharedIPad|Booliano|Isso indica se o dispositivo deve ser registrado em um modo que habilita cenários de vários usuários. Aplicável somente em iPads compartilhados.|
|companyPortalVppTokenId|Cadeia de Caracteres|Se definido, indica qual token Vpp deve ser usado para implantar o Portal da Empresa w/ licenciamento de dispositivo. 'enableAuthenticationViaCompanyPortal' deve ser definido para que essa propriedade seja definida.|
|enableSingleAppEnrollmentMode|Booliano|Instrui o dispositivo a habilitar o modo de aplicativo único e aplicar o bloqueio de aplicativo durante o registro. O padrão é false. 'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidos para que essa propriedade seja definida.|
|homeButtonScreenDisabled|Booliano|Indica se a tela de confidencialidade do botão página inicial está desabilitada|
|iMessageAndFaceTimeScreenDisabled|Booliano|Indica se a tela iMessage e FaceTime está desabilitada|
|onBoardingScreenDisabled|Booliano|Indica se a tela de configuração de integração está desabilitada|
|simSetupScreenDisabled|Boolean|Indica se a tela SIMSetup está desabilitada|
|softwareUpdateScreenDisabled|Booliano|Indica se a tela de atualização de sofware obrigatória está desabilitada|
|watchMigrationScreenDisabled|Booliano|Indica se a tela de migração do relógio está desabilitada|
|appearanceScreenDisabled|Boolean|Indica se a tela do Apperance está desabilitada|
|expressLanguageScreenDisabled|Booliano|Indica se a tela express language está desabilitada|
|preferredLanguageScreenDisabled|Booliano|Indica se a tela idioma preferencial está desabilitada|
|deviceToDeviceMigrationDisabled|Booliano|Indica se a Migração de Dispositivo para Dispositivo está desabilitada|
|welcomeScreenDisabled|Booliano|Indica se a tela Weclome está desabilitada|
|passCodeDisabled|Booliano|Indica se o painel de configuração de senha está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|restoreCompletedScreenDisabled|Booliano|Indica se a tela Weclome está desabilitada|
|updateCompleteScreenDisabled|Booliano|Indica se a tela Weclome está desabilitada|
|forceTemporarySession|Boolean|Indica se as sessões temporárias estão habilitadas|
|temporarySessionTimeoutInSeconds|Int32|Indica o tempo limite da sessão temporária|
|userSessionTimeoutInSeconds|Int32|Indica o tempo limite da sessão temporária|
|passcodeLockGracePeriodInSeconds|Int32|Indica o tempo limite antes que a tela bloqueada exija que o usuário insira a passagem do dispositivo para desbloqueá-la|
|carrierActivationUrl|Cadeia de Caracteres|URL da operadora para ativar o eSIM do dispositivo.|
|userlessSharedAadModeEnabled|Booliano|Indica que esse dispositivo apple é designado para dar suporte a cenários de "modo de dispositivo compartilhado". Isso é diferente do cenário de "iPad compartilhado". Ver https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-shared-ios|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 2377

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2426

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```




