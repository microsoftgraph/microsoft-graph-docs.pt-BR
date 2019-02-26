---
title: Tipo de recurso sharedPCConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69bae063082a49bb46b6bdc0e6e3364cbd2a83e5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152630"
---
# <a name="sharedpcconfiguration-resource-type"></a>Tipo de recurso sharedPCConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

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
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|Especifica como as contas são gerenciadas em um PC compartilhado. Aplica-se somente quando disableAccountManager é false.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|Indica que tipos de contas podem ser usadas em um PC compartilhado. Os valores possíveis são: `notConfigured`, `guest`, `domain`.|
|localStorage|[habilitação](../resources/intune-shared-enablement.md)|Especifica se o armazenamento local é permitido em um PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|allowLocalStorage|Boolean|Especifica se o armazenamento local é permitido em um PC compartilhado.|
|setAccountmanager|[habilitação](../resources/intune-shared-enablement.md)|Desabilita o gerente de contas para o modo de PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableAccountManager|Boolean|Desabilita o gerente de contas para o modo de PC compartilhado.|
|setEduPolicies|[habilitação](../resources/intune-shared-enablement.md)|Especifica se as políticas de ambiente de educação de computador compartilhado padrão devem ser habilitadas/desabilitadas/não configuradas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableEduPolicies|Boolean|Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.|
|setPowerPolicies|[habilitação](../resources/intune-shared-enablement.md)|Especifica se as políticas de energia padrão do computador compartilhado devem ser ativadas/desativadas. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disablePowerPolicies|Boolean|Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.|
|signInOnResume|[habilitação](../resources/intune-shared-enablement.md)|Especifica o requisito para entrar sempre que o dispositivo é ativado do modo de suspensão. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableSignInOnResume|Booliano|Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.|
|enabled|Boolean|Habilita o modo de PC compartilhado e aplica as políticas de PC compartilhadas.|
|idleTimeBeforeSleepInSeconds|Int32|Especifica o tempo em segundos que um dispositivo deve ficar ocioso antes de o PC entrar em suspensão. Definir esse valor como 0 impede que o tempo limite de suspensão ocorra.|
|kioskAppDisplayName|String|Especifica o texto de exibição para a conta mostrada na tela de entrada que inicializa o aplicativo especificado por SetKioskAppUserModelId. Aplicável somente quando KioskAppUserModelId está definido.|
|kioskAppUserModelId|String|Especifica a ID do modelo de usuário do aplicativo para uso com acesso atribuído.|
|maintenanceStartTime|TimeOfDay|Especifica o horário de início diário da hora de manutenção.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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
  "maintenanceStartTime": "String (time of day)"
}
```




