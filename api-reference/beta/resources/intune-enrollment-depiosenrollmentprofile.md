---
title: Tipo de recurso depIOSEnrollmentProfile
description: O recurso DepIOSEnrollmentProfile representa um perfil de registro do DEP (Programa de Registro de Dispositivo) da Apple específico para a configuração do iOS. Esse tipo de perfil deve ser atribuído aos números de série do DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio do DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2f8055409be315ffd1b5ba2fb3686655b334ba8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210749"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Tipo de recurso depIOSEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso DepIOSEnrollmentProfile representa um perfil de registro do DEP (Programa de Registro de Dispositivo) da Apple específico para a configuração do iOS. Esse tipo de perfil deve ser atribuído aos números de série do DEP da Apple antes que os dispositivos correspondentes possam se registrar por meio do DEP.


Herda [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[Coleção de depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Listar propriedades e relações dos [objetos depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Obter depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Ler propriedades e relações do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Criar depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Crie um novo [objeto depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Excluir depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Nenhuma|Exclui um [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Atualizar depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Atualize as propriedades de [um objeto depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Cadeia de caracteres|Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|descrição|Cadeia de caracteres|Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de Caracteres|URL do ponto de extremidade de configuração a ser usada para Registro Herdado do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booliano|Indica a autenticação com o Assistente de Configuração da Apple em vez de Portal da Empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indica que o Portal da Empresa é necessário em dispositivos registrados do assistente de configuração Herdados do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|Modo supervisionado, True para habilitar; caso contrário, false. Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais. Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Cadeia de Caracteres|Informações do departamento de suporte [herdadas de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Booliano|Indica se o perfil é obrigatório Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|Indica se o painel de configuração do serviço local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Cadeia de Caracteres|Suporte ao número de telefone [Herdado de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Booliano|Indica se o painel de instalação restaurar está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|Indica se o painel de instalação da ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Booliano|Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|Indica se o painel de configuração da ID de toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|Indica se o painel de instalação da siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Booliano|Indica se o painel de configuração de diagnóstico está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
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
|onBoardingScreenDisabled|Boolean|Indica se a tela de configuração de integração está desabilitada|
|simSetupScreenDisabled|Booliano|Indica se a tela SIMSetup está desabilitada|
|softwareUpdateScreenDisabled|Booliano|Indica se a tela de atualização de sofware obrigatória está desabilitada|
|watchMigrationScreenDisabled|Boolean|Indica se a tela de migração do relógio está desabilitada|
|appearanceScreenDisabled|Booliano|Indica se a tela do Apperance está desabilitada|
|expressLanguageScreenDisabled|Booliano|Indica se a tela express language está desabilitada|
|preferredLanguageScreenDisabled|Booliano|Indica se a tela idioma preferencial está desabilitada|
|deviceToDeviceMigrationDisabled|Booliano|Indica se a Migração de Dispositivo para Dispositivo está desabilitada|
|welcomeScreenDisabled|Booliano|Indica se a tela Weclome está desabilitada|
|passCodeDisabled|Booliano|Indica se o painel de configuração de senha está desabilitado|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado|
|restoreCompletedScreenDisabled|Boolean|Indica se a tela Weclome está desabilitada|
|updateCompleteScreenDisabled|Booliano|Indica se a tela Weclome está desabilitada|
|forceTemporarySession|Boolean|Indica se as sessões temporárias estão habilitadas|
|temporarySessionTimeoutInSeconds|Int32|Indica o tempo limite da sessão temporária|
|userSessionTimeoutInSeconds|Int32|Indica o tempo limite da sessão temporária|
|passcodeLockGracePeriodInSeconds|Int32|Indica o tempo limite antes que a tela bloqueada exija que o usuário insira a passagem do dispositivo para desbloqueá-la|
|carrierActivationUrl|Cadeia de Caracteres|URL da operadora para ativar o eSIM do dispositivo.|
|userlessSharedAadModeEnabled|Booliano|Indica que esse dispositivo apple é designado para dar suporte a cenários de "modo de dispositivo compartilhado". Isso é diferente do cenário de "iPad compartilhado". Ver https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-shared-ios|

## <a name="relationships"></a>Relações
Nenhuma

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
  "carrierActivationUrl": "String",
  "userlessSharedAadModeEnabled": true
}
```




