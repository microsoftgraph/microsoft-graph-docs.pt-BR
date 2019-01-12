---
title: Atualizar depIOSEnrollmentProfile
description: Atualize as propriedades de um objeto depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cfbae59533112d69d4616f77d2dbeb79a6361332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935959"
---
# <a name="update-depiosenrollmentprofile"></a>Atualizar depIOSEnrollmentProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualize as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
No corpo da solicitação, fornece uma representação JSON para o objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Cadeia de caracteres|Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Cadeia de caracteres|Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Booliano|Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Cadeia de caracteres|Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Booliano|Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Booliano|Modo supervisionado, True para habilitar, false caso contrário. Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais. Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Cadeia de caracteres|Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|passCodeDisabled|Booliano|Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Booliano|Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Booliano|Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Cadeia de caracteres|Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Booliano|Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Booliano|Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Booliano|Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Booliano|Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Booliano|Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Booliano|Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|zoomDisabled|Booliano|Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Booliano|Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Booliano|Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica a modo de emparelhamento de iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para configurador da Apple|
|restoreFromAndroidDisabled|Booliano|Indica se a restauração do Android está desabilitada|
|awaitDeviceConfiguredConfirmation|Booliano|Indica se o dispositivo será necessário aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Especifica o número máximo de usuários que podem utilizar um iPad compartilhado. Só é aplicável no modo compartilhado iPad.|
|enableSharedIPad|Booliano|Isso indica se o dispositivo é registrado em um modo que permite que vários cenários de usuário. Só é aplicável no compartilhados iPads.|
|companyPortalVppTokenId|Cadeia de caracteres|Se definido, que indica qual token Vpp deve ser usado para implantar o Portal da empresa c / licenciamento do dispositivo. 'enableAuthenticationViaCompanyPortal' deve ser definida para que essa propriedade ser definida.|
|enableSingleAppEnrollmentMode|Booliano|Informa o dispositivo para habilitar o modo de aplicativo único e aplicar o app-lock durante o registro. O padrão é false. 'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidas para que essa propriedade ser definida.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1267

{
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
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
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
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
  "enableSingleAppEnrollmentMode": true
}
```





