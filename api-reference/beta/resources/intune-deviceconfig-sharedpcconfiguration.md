---
title: Tipo de recurso sharedPCConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4e4a8806a19f9fd0563f05b8d2a75b359f7e0c6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276676"
---
# <a name="sharedpcconfiguration-resource-type"></a>Tipo de recurso sharedPCConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sharedPCConfigurations](../api/intune-deviceconfig-sharedpcconfiguration-list.md)|Coleção [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Lista propriedades e relações dos objetos [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Obter sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-get.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Propriedades de leitura e relações do objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Criar sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-create.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Cria um novo objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Excluir sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-delete.md)|Nenhum|Exclui um [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|
|[Atualizar sharedPCConfiguration](../api/intune-deviceconfig-sharedpcconfiguration-update.md)|[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)|Atualiza as propriedades de um objeto [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para essa política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para essa política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|Especifica como as contas são gerenciadas em um PC compartilhado. Aplica-se somente quando disableAccountManager é false.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|Indica que tipos de contas podem ser usadas em um PC compartilhado. Os valores possíveis são: `notConfigured`, `guest`, `domain`.|
|localStorage|[habilitação](../resources/intune-shared-enablement.md)|Especifica se o armazenamento local é permitido em um PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|allowLocalStorage|Boolean|Especifica se o armazenamento local é permitido em um PC compartilhado.|
|setaccountmanager|[habilitação](../resources/intune-shared-enablement.md)|Desabilita o gerente de contas para o modo de PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableAccountManager|Boolean|Desabilita o gerente de contas para o modo de PC compartilhado.|
|setEduPolicies|[habilitação](../resources/intune-shared-enablement.md)|Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableEduPolicies|Boolean|Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.|
|setPowerPolicies|[habilitação](../resources/intune-shared-enablement.md)|Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disablePowerPolicies|Boolean|Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.|
|signInOnResume|[habilitação](../resources/intune-shared-enablement.md)|Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableSignInOnResume|Boolean|Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.|
|enabled|Boolean|Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.|
|idleTimeBeforeSleepInSeconds|Int32|Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão. Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.|
|kioskAppDisplayName|String|Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId. Aplicável somente quando KioskAppUserModelId está definido.|
|kioskAppUserModelId|String|Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.|
|maintenanceStartTime|TimeOfDay|Especifica o horário de início diário da hora de manutenção.|
|fastFirstSignIn|[habilitação](../resources/intune-shared-enablement.md)|Especifica se a conexão automática de novas contas não administrativas do Azure AD para contas locais de candidatos pré-configuradas. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "String",
    "cacheAccountsAboveDiskFreePercentage": 1024,
    "inactiveThresholdDays": 1024,
    "removeAccountsBelowDiskFreePercentage": 1024
  },
  "allowedAccounts": "String",
  "localStorage": "String",
  "allowLocalStorage": true,
  "setAccountManager": "String",
  "disableAccountManager": true,
  "setEduPolicies": "String",
  "disableEduPolicies": true,
  "setPowerPolicies": "String",
  "disablePowerPolicies": true,
  "signInOnResume": "String",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 1024,
  "kioskAppDisplayName": "String",
  "kioskAppUserModelId": "String",
  "maintenanceStartTime": "String (time of day)",
  "fastFirstSignIn": "String"
}
```




