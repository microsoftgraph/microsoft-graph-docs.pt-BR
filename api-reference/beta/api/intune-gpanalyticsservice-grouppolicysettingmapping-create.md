---
title: Criar groupPolicySettingMapping
description: Crie um novo objeto groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd2fd96004b5d8d7b36437eb3114472f2f60a6ff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340309"
---
# <a name="create-grouppolicysettingmapping"></a>Criar groupPolicySettingMapping

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicySettingMapping.

A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicySettingMapping.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|parentId|String|ID pai da configuração de política de grupo.|
|childIdList|Coleção String|Lista de IDs Filho da configuração de política de grupo.|
|settingName|Cadeia de caracteres|O nome dessa configuração de política de grupo.|
|settingValue|String|O valor dessa configuração de política de grupo.|
|settingValueType|String|O tipo de valor dessa configuração de política de grupo.|
|settingDisplayName|String|O nome de exibição dessa configuração de política de grupo.|
|settingDisplayValue|String|O valor de exibição dessa configuração de política de grupo.|
|settingDisplayValueType|String|O tipo de valor de exibição dessa configuração de política de grupo.|
|settingValueDisplayUnits|String|As unidades de exibição desse valor de configuração de política de grupo|
|settingCategory|String|A categoria em que a configuração da política de grupo está.|
|mdmCspName|String|O nome CSP para o que a configuração da política de grupo mapeia.|
|mdmSettingUri|String|O URI CSP do MDM para o que a política de grupo mapeia.|
|mdmMinimumOSVersion|Int32|A versão mínima do sistema operacional compatível com essa configuração mdm.|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|O tipo de configuração (segurança ou admx) da Política de Grupo. Os valores possíveis são: `unknown` , , , , , , , , `policy` `account` `securityOptions` `userRightsAssignment` `auditSetting` `windowsFirewallSettings` `appLockerRuleCollection` `dataSourcesSettings` `devicesSettings` `driveMapSettings` `environmentVariables` `filesSettings` `folderOptions` , `folders` `iniFiles` `internetOptions` `localUsersAndGroups` `networkOptions` `networkShares` `ntServices` `powerOptions` `printers` `regionalOptionsSettings` `registrySettings` `scheduledTasks` `shortcutSettings` `startMenuSettings`|
|isMdmSupported|Boolean|Indica se a configuração é suportada pelo Intune ou não|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Indica se a configuração é suportada no Mdm ou não. Os valores possíveis são: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|O escopo da configuração. Os valores possíveis são: `unknown`, `device`, `user`.|
|intuneSettingUriList|Coleção de cadeias de caracteres|A lista de URIs de configuração do Intune para as configurações de política de grupo mapeia para|
|intuneSettingDefinitionId|String|A ID de Definição de Configuração do Intune|
|admxSettingDefinitionId|String|ID da Política de Grupo Admx|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings
Content-type: application/json
Content-length: 1023

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1072

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```




