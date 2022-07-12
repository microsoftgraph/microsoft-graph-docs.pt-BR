---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11fb6586a2928f47e076cdd5240c2287d3e94a32
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733539"
---
# <a name="update-windows81generalconfiguration"></a>Atualizar windows81GeneralConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|applyOnlyToWindows81|Boolean|Valor que indica se esta política se aplica somente ao Windows 8.1. Essa propriedade é somente leitura.|
|browserBlockAutofill|Boolean|Indica se o preenchimento automático deve ou não ser bloqueado.|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.|
|browserBlockEnterpriseModeAccess|Boolean|Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.|
|browserBlockJavaScript|Boolean|Indica se o usuário será ou não impedido de usar JavaScript.|
|browserBlockPlugins|Boolean|Indica se os plug-ins devem ou não ser bloqueados.|
|browserBlockPopups|Boolean|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|browserBlockSendingDoNotTrackHeader|Boolean|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.|
|browserRequireSmartScreen|Boolean|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|browserEnterpriseModeSiteListLocation|String|O local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|O nível de segurança da Internet. Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|O nível de segurança da Intranet. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|String|O local do relatório de registro em log.|
|browserRequireHighSecurityForRestrictedSites|Boolean|Indica se a alta segurança para sites restritos deve ou não ser exigida.|
|browserRequireFirewall|Boolean|Indica se um firewall deve ou não ser exigido.|
|browserRequireFraudWarning|Boolean|Indica se um aviso de fraude deve ou não ser exigido.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|O nível de segurança de sites confiáveis. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Boolean|Indica se o roaming de dados deve ou não ser bloqueado.|
|diagnosticsBlockDataSubmission|Boolean|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|passwordBlockPicturePasswordAndPin|Boolean|Indica se o usuário será ou não impedido de usar senha com imagens ou pin.|
|passwordExpirationDays|Int32|Expiração da senha em dias.|
|passwordMinimumLength|Int32|O comprimento mínimo da senha.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica.|
|storageRequireDeviceEncryption|Boolean|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|updatesRequireAutomaticUpdates|Boolean|Indica se as atualizações automáticas devem ou não ser exigidas.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|As configurações de controle da conta do usuário. Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|String|A URL das pastas de trabalho|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





