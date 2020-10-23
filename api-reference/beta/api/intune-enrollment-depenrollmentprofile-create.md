---
title: Criar depEnrollmentProfile
description: Criar um novo objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8157e164113de27bd0761bbf8a48bae380c2e42
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706664"
---
# <a name="create-depenrollmentprofile"></a>Criar depEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Criar um novo objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto depEnrollmentProfile.

A tabela a seguir mostra as propriedades que são necessárias ao criar depEnrollmentProfile.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|Enableauthenticationviacompanyportal foi adicionada|Boolean|Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa. Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Booliano|Indica se este é o perfil padrão|
|supervisedModeEnabled|Boolean|Modo supervisionado, true para habilitar, caso contrário, false. Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.|
|supportDepartment|String|Informações do departamento de suporte|
|passCodeDisabled|Boolean|Indica se o painel de configuração de senha está desabilitado|
|IsMandatory|Boolean|Indica se o perfil é obrigatório|
|locationDisabled|Boolean|Indica se o painel de instalação do serviço de localização está desabilitado|
|supportPhoneNumber|String|Número de telefone de suporte|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Indica o modo de emparelhamento do iTunes. Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Boolean|Indica se a opção de remoção de perfil está desabilitada|
|managementCertificates|coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Certificados de gerenciamento para o Apple Configurator|
|restoreBlocked|Boolean|Indica se o painel de configuração de restauração está bloqueado|
|restoreFromAndroidDisabled|Boolean|Indica se a restauração do Android está desabilitada|
|appleIdDisabled|Boolean|Indica se o painel de configuração de ID da Apple está desabilitado|
|termsAndConditionsDisabled|Boolean|Indica se o painel de configuração ' termos e condições ' está desabilitado|
|touchIdDisabled|Boolean|Indica se o painel de configuração de ID de toque está desabilitado|
|applePayDisabled|Boolean|Indica se o painel de configuração de pagamento da Apple está desabilitado|
|zoomDisabled|Boolean|Indica se o painel de configuração de zoom está desabilitado|
|siriDisabled|Boolean|Indica se o painel de configuração do Siri está desabilitado|
|diagnosticsDisabled|Boolean|Indica se o painel de configuração de diagnóstico está desabilitado|
|macOSRegistrationDisabled|Boolean|Indica se o registro do Mac OS está desabilitado|
|macOSFileVaultDisabled|Boolean|Indica se o compartimento de arquivos do Mac OS está desabilitado|
|awaitDeviceConfiguredConfirmation|Boolean|Indica se o dispositivo deverá aguardar a confirmação configurada|
|sharedIPadMaximumUserCount|Int32|Isso especifica o número máximo de usuários que podem usar um iPad compartilhado. Aplicável somente no modo iPad compartilhado.|
|enableSharedIPad|Boolean|Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários. Aplicável somente no iPads compartilhado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```





