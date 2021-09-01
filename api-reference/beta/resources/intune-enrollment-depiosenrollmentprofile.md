---
title: Tipo de recurso de depIOSEnrollmentProfile
description: O recurso DepIOSEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP) específico da configuração do iOS. Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9b500eac7d6a1e4d0dcc5346dee191d36ff1f8f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783915"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Tipo de recurso de depIOSEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepIOSEnrollmentProfile representa um perfil de registro do Programa de Registro de Dispositivo Apple (DEP) específico da configuração do iOS. Esse tipo de perfil deve ser atribuído aos números de série de DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio de DEP.


Herda [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[Coleção de depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Listar propriedades e relações dos [objetos depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)|
|[Obter depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Leia propriedades e relações do [objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)|
|[Criar depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Crie um novo [objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)|
|[Excluir depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Nenhum(a)|Exclui um [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Atualizar depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Atualize as propriedades de [um objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Cadeia de caracteres|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|descrição|Cadeia de caracteres|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boleano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de caracteres|URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boleano|Indica a autenticação com o Assistente de Instalação da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boleano|Indica que a Portal da Empresa é necessária em dispositivos inscritos do assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boleano|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Cadeia de caracteres|Informações do departamento de suporte Herdadas [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Boleano|Indica se o perfil é obrigatório Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Booliano|Indica se o painel de configuração do serviço de local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Cadeia de caracteres|Número de telefone de suporte Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boleano|Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boleano|Indica se o painel restaurar instalação está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boleano|Indica se o painel de configuração de ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boleano|Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boleano|Indica se o painel de configuração de id por toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boleano|Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boleano|Indica se o painel de configuração de siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boleano|Indica se o painel de configuração de diagnósticos está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boleano|Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boleano|Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boleano|Indica se a configuração do tempo de tempo de tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Cadeia de caracteres|Define um padrão literal ou de nome. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Boleano|URL para logon do assistente de instalação Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica o modo de emparelhamento do iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para o Apple Configurator|
|restoreFromAndroidDisabled|Boleano|Indica se a restauração do Android está desabilitada|
|awaitDeviceConfiguredConfirmation|Boleano|Indica se o dispositivo precisará aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Isso especifica o número máximo de usuários que podem usar um iPad. Aplicável somente no modo iPad compartilhado.|
|enableSharedIPad|Boleano|Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários. Aplicável somente em iPads compartilhados.|
|companyPortalVppTokenId|Cadeia de caracteres|Se definido, indica qual token Vpp deve ser usado para implantar o Portal da Empresa w/device. 'enableAuthenticationViaCompanyPortal' deve ser definido para que essa propriedade seja definida.|
|enableSingleAppEnrollmentMode|Boleano|Informa ao dispositivo para habilitar o modo de aplicativo único e aplicar o bloqueio de aplicativo durante o registro. O padrão é falso. 'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidos para que essa propriedade seja definida.|
|homeButtonScreenDisabled|Boleano|Indica se a tela de sensibilidade do botão inicial está desabilitada|
|iMessageAndFaceTimeScreenDisabled|Boleano|Indica se a tela iMessage e FaceTime está desabilitada|
|onBoardingScreenDisabled|Boleano|Indica se a tela de instalação de integração está desabilitada|
|simSetupScreenDisabled|Boleano|Indica se a tela SIMSetup está desabilitada|
|softwareUpdateScreenDisabled|Boleano|Indica se a tela de atualização de sofware obrigatória está desabilitada|
|watchMigrationScreenDisabled|Boleano|Indica se a tela de migração do relógio está desabilitada|
|appearanceScreenDisabled|Boleano|Indica se a tela do Apperance está desabilitada|
|expressLanguageScreenDisabled|Boleano|Indica se a tela linguagem expressa está desabilitada|
|preferredLanguageScreenDisabled|Boleano|Indica se a tela de idioma preferencial está desabilitada|
|deviceToDeviceMigrationDisabled|Boleano|Indica se a migração de dispositivo para dispositivo está desabilitada|
|welcomeScreenDisabled|Boleano|Indica se a tela Weclome está desabilitada|
|passCodeDisabled|Boleano|Indica se o painel de configuração senha está desabilitado|
|zoomDisabled|Boleano|Indica se o painel de configuração de zoom está desabilitado|
|restoreCompletedScreenDisabled|Boleano|Indica se a tela Weclome está desabilitada|
|updateCompleteScreenDisabled|Boleano|Indica se a tela Weclome está desabilitada|
|forceTemporarySession|Boleano|Indica se as sessões temporárias estão habilitadas|
|temporarySessionTimeoutInSeconds|Int32|Indica o tempo de tempo de sessão temporária|
|userSessionTimeoutInSeconds|Int32|Indica o tempo de tempo de sessão temporária|
|passcodeLockGracePeriodInSeconds|Int32|Indica o tempo-de-tempo antes da tela bloqueada exigir que o usuário insira a passagem do dispositivo para desbloqueá-la|
|carrierActivationUrl|Cadeia de caracteres|URL da operadora para ativar o eSIM do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
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
  "temporarySessionTimeoutInSeconds": 1024,
  "userSessionTimeoutInSeconds": 1024,
  "passcodeLockGracePeriodInSeconds": 1024,
  "carrierActivationUrl": "String"
}
```



