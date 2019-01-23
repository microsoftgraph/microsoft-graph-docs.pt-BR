---
title: Atualizar androidWorkProfileGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0cec0b230b9e8735b5071920ccba8639ea58de2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410032"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a>Atualizar androidWorkProfileGeneralDeviceConfiguration

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualize as propriedades de um objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|passwordBlockFingerprintUnlock|Boolean|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockTrustAgents|Boolean|Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 0 a 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número permitido de falhas de entrada antes da redefinição de fábrica. Valores válidos 1 a 16|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Tipo de dados de compartilhamento que é permitido. Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolean|Indica se deve ou não bloquear notificações de dispositivo bloqueado.|
|workProfileBlockAddingAccounts|Boolean|Impedir que os usuários de adicionar/remover contas no perfil de trabalho.|
|workProfileBluetoothEnableContactSharing|Boolean|Permitir que os dispositivos bluetooth acessar contatos da empresa.|
|workProfileBlockScreenCapture|Boolean|Captura de tela de bloqueio no perfil de trabalho.|
|workProfileBlockCrossProfileCallerId|Boolean|Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.|
|workProfileBlockCamera|Boolean|Câmera de perfil de trabalho de bloco.|
|workProfileBlockCrossProfileContactsSearch|Boolean|Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.|
|workProfileBlockCrossProfileCopyPaste|Boolean|Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Boolean|Indica se o bloqueio da impressão digital ou não desbloquear para o perfil de trabalho.|
|workProfilePasswordBlockTrustAgents|Boolean|Indica se deve ou não bloquear bloqueio inteligente e outros operadores de confiabilidade para o perfil de trabalho.|
|workProfilePasswordExpirationDays|Int32|Número de dias até a senha do perfil de trabalho expira. Valores válidos de 1 a 365|
|workProfilePasswordMinimumLength|Int32|Comprimento mínimo da senha do perfil de trabalho. Valores válidos de 4 a 16|
|workProfilePasswordMinNumericCharacters|Int32|Número mínimo de caracteres numéricos necessários em senha do perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Número mínimo de caracteres não alfabéticos necessários em senha de perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinLetterCharacters|Int32|Número mínimo de caracteres de carta necessários em senha de perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Número mínimo de caracteres minúscula necessários em senha de perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Número mínimo de caracteres de maiusculas necessários em senha de perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinSymbolCharacters|Int32|Número mínimo de símbolos necessários em senha de perfil de trabalho. Valores válidos 1 a 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Número de senhas anteriores de perfil de trabalho para bloquear. Valores válidos de 0 a 24|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada. Valores válidos 1 a 16|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Tipo de senha de perfil de trabalho que é necessário. Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Boolean|A senha é necessária ou não para o perfil de trabalho|
|securityRequireVerifyApps|Boolean|Exige que o recurso de verificação de aplicativos Android esteja ativado.|
|vpnAlwaysOnPackageIdentifier|String|Habilite o modo de bloqueio para VPN sempre ativada.|
|vpnEnableAlwaysOnLockdownMode|Boolean|Habilite o modo de bloqueio para VPN sempre ativada.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




