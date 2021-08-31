---
title: Atualizar windowsIdentityProtectionConfiguration
description: Atualize as propriedades de um objeto windowsIdentityProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea9f6d879cab6bcb3673e68327ab91181457f9de
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796387"
---
# <a name="update-windowsidentityprotectionconfiguration"></a>Atualizar windowsIdentityProtectionConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto windowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto windowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|useSecurityKeyForSignin|Boleano|Valor booleano usado para habilitar a Windows Hello de segurança como uma credencial de logon.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boleano|Valor booleano usado para habilitar a anti-spoofing aprimorado para reconhecimento de recursos faciais Windows Hello face autenticação.|
|pinMinimumLength|Int32|Valor inteiro que define o número mínimo de caracteres necessário para o pin Windows Hello para Empresas. Os valores válidos são de 4 a 127 inclusive e menor ou igual ao valor definido para o PIN máximo. Valores válidos de 4 a 127|
|pinMaximumLength|Int32|Valor inteiro que define o número máximo de caracteres permitidos para o PIN de trabalho. Os valores válidos são de 4 a 127 inclusive e maiores ou iguais ao valor definido para o PIN mínimo. Valores válidos de 4 a 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Esse valor configura o uso de caracteres maiúsculas no pin Windows Hello para Empresas. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Esse valor configura o uso de caracteres minúsculos no pin Windows Hello para Empresas. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Controla a capacidade de usar caracteres especiais no pin Windows Hello para Empresas. Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinExpirationInDays|Int32|Valor inteiro especifica o período (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere. Os valores válidos são de 0 a 730 inclusive. Valores válidos de 0 a 730|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários usem PINs anteriores. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem. Se definido como 0, os PINs anteriores não serão armazenados. O histórico de PIN não é preservado por meio de uma redefinição de PIN. Valores válidos de 0 a 50|
|pinRecoveryEnabled|Boleano|Valor booleano que permite que um usuário altere seu PIN usando o Windows Hello de recuperação de PIN comercial.|
|securityDeviceRequired|Booliano|Controla se é necessário um TPM (Trusted Platform Module) para provisionamento Windows Hello para Empresas. Um TPM fornece um benefício adicional de segurança, já que os dados armazenados nele não podem ser usados em outros dispositivos. Se definido como False, todos os dispositivos podem provisionar Windows Hello para Empresas, mesmo que não haja um TPM usável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa ao PIN Windows Hello para Empresas.  Se definido como False, gestos biométricos não são permitidos. Os usuários ainda devem configurar um PIN como backup em caso de falhas.|
|useCertificatesForOnPremisesAuthEnabled|Boleano|Valor booleano que permite Windows Hello para Empresas usar certificados para autenticar recursos locais.|
|windowsHelloForBusinessBlocked|Boolean|Valor booleano que bloqueia Windows Hello para Empresas como um método para entrar no Windows.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```



