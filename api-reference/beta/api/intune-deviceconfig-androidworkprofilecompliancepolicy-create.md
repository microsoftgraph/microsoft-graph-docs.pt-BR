---
title: Criar androidWorkProfileCompliancePolicy
description: Crie um novo objeto androidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98af8dd087f7cf0bbe8703b4f86f09776df807e8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58822030"
---
# <a name="create-androidworkprofilecompliancepolicy"></a>Criar androidWorkProfileCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto androidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto androidWorkProfileCompliancePolicy.

A tabela a seguir mostra as propriedades que são necessárias ao criar o androidWorkProfileCompliancePolicy.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância entity. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|passwordRequired|Boolean|Exige uma senha para desbloquear o dispositivo.|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|Tipo de caracteres em senha. Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 1 a 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número de falhas de login permitidas antes da redefinição de fábrica. Valores válidos de 1 a 16|
|securityPreventInstallAppsFromUnknownSources|Boolean|Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.|
|securityDisableUsbDebugging|Boolean|Desabilite a depuração USB em dispositivos Android.|
|securityRequireVerifyApps|Boolean|Exige que o recurso de verificação de aplicativos Android esteja ativado.|
|deviceThreatProtectionEnabled|Boolean|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|advancedThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|O MDATP exige nível mínimo de risco da Proteção Contra Ameaças Móveis para relatar o não-atendimento. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|securityBlockJailbrokenDevices|Boolean|Os dispositivos não devem ser violados ou com modificações root.|
|osMinimumVersion|String|Versão mínima do Android.|
|osMaximumVersion|String|Versão máxima do Android.|
|minAndroidSecurityPatchLevel|String|Nível mínimo de patch de segurança Android.|
|storageRequireEncryption|Boolean|Exige criptografia em dispositivos Android.|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolean|Exige que o dispositivo passe na verificação de integridade básica SafetyNet.|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolean|Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.|
|securityRequireGooglePlayServices|Boolean|Exige que os Google Play Services sejam instalados e habilitados no dispositivo.|
|securityRequireUpToDateSecurityProviders|Boolean|Exige que o dispositivo tenha provedores de segurança atualizados. O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.|
|securityRequireCompanyPortalAppIntegrity|Boolean|Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.|
|securityRequiredAndroidSafetyNetEvaluationType|[androidSafetyNetEvaluationType](../resources/intune-deviceconfig-androidsafetynetevaluationtype.md)|Exigir um tipo de avaliação SafetyNet específico para conformidade. Os valores possíveis são: `basic` e `hardwareBacked`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1421

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1593

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```



