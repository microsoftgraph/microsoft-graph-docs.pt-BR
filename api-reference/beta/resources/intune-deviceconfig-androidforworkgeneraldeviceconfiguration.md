---
title: tipo de recurso de androidForWorkGeneralDeviceConfiguration
description: Configuração de dispositivo gerais Android para trabalho.
author: tfitzmac
ms.openlocfilehash: 3b8aa84ea4a59487c2d5889bb179ad0615663e24
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329439"
---
# <a name="androidforworkgeneraldeviceconfiguration-resource-type"></a>tipo de recurso de androidForWorkGeneralDeviceConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração de dispositivo gerais Android para trabalho.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidForWorkGeneralDeviceConfigurations](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-list.md)|coleção [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .|
|[Obter androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-get.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .|
|[Criar androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-create.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Crie um novo objeto de [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .|
|[Excluir androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-delete.md)|Nenhum|Exclui um [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).|
|[Atualizar androidForWorkGeneralDeviceConfiguration](../api/intune-deviceconfig-androidforworkgeneraldeviceconfiguration-update.md)|[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)|Atualize as propriedades de um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Propriedades
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
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número permitido de falhas de entrada antes da redefinição de fábrica. Valores válidos de 4 a 11|
|passwordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidForWorkCrossProfileDataSharingType](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|Tipo de dados de compartilhamento que é permitido. Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Boolean|Indica se deve ou não bloquear notificações de dispositivo bloqueado.|
|workProfileBlockAddingAccounts|Boolean|Impedir que os usuários de adicionar/remover contas no perfil de trabalho.|
|workProfileBluetoothEnableContactSharing|Boolean|Permitir que os dispositivos bluetooth acessar contatos da empresa.|
|workProfileBlockScreenCapture|Boolean|Captura de tela de bloqueio no perfil de trabalho.|
|workProfileBlockCrossProfileCallerId|Boolean|Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.|
|workProfileBlockCamera|Boolean|Câmera de perfil de trabalho de bloco.|
|workProfileBlockCrossProfileContactsSearch|Boolean|Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.|
|workProfileBlockCrossProfileCopyPaste|Boolean|Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.|
|workProfileDefaultAppPermissionPolicy|[androidForWorkDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
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
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada. Valores válidos de 4 a 11|
|workProfilePasswordRequiredType|[androidForWorkRequiredPasswordType](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|Tipo de senha de perfil de trabalho que é necessário. Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Boolean|A senha é necessária ou não para o perfil de trabalho|
|securityRequireVerifyApps|Boolean|Exige que o recurso de verificação de aplicativos Android esteja ativado.|
|vpnAlwaysOnPackageIdentifier|String|Habilite o modo de bloqueio para VPN sempre ativada.|
|vpnEnableAlwaysOnLockdownMode|Boolean|Habilite o modo de bloqueio para VPN sempre ativada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "workProfileDataSharingType": "String",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "String",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1024,
  "workProfilePasswordMinimumLength": 1024,
  "workProfilePasswordMinNumericCharacters": 1024,
  "workProfilePasswordMinNonLetterCharacters": 1024,
  "workProfilePasswordMinLetterCharacters": 1024,
  "workProfilePasswordMinLowerCaseCharacters": 1024,
  "workProfilePasswordMinUpperCaseCharacters": 1024,
  "workProfilePasswordMinSymbolCharacters": 1024,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "workProfilePasswordPreviousPasswordBlockCount": 1024,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 1024,
  "workProfilePasswordRequiredType": "String",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnEnableAlwaysOnLockdownMode": true
}
```





