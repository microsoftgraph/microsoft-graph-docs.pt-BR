---
title: Tipo de recurso sharedPCConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso sharedPCConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61d7c1214f629673f2b738d705c055b3020f0ed5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415107"
---
# <a name="sharedpcconfiguration-resource-type"></a>Tipo de recurso sharedPCConfiguration

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountManagerPolicy|[sharedPCAccountManagerPolicy](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|Especifica como as contas são gerenciadas em um PC compartilhado. Aplica-se somente quando disableAccountManager é false.|
|allowedAccounts|[sharedPCAllowedAccountType](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|Indica que tipos de contas podem ser usadas em um PC compartilhado. Os valores possíveis são: `notConfigured`, `guest`, `domain`.|
|localStorage|[habilitação] (.. /Resources/Intune-Shared-Enablement
.MD)|Especifica se o armazenamento local é permitido em um PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|allowLocalStorage|Boolean|Especifica se o armazenamento local é permitido em um PC compartilhado.|
|setAccountManager|[habilitação] (.. /Resources/Intune-Shared-Enablement
.MD)|Desabilita o gerente de contas para o modo de PC compartilhado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableAccountManager|Boolean|Desabilita o gerente de contas para o modo de PC compartilhado.|
|setEduPolicies|[habilitação] (.. /Resources/Intune-Shared-Enablement
.MD)|Especifica se as políticas de ambiente de educação de PC compartilhada padrão devem ser ativado/desativado/não são configuradas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableEduPolicies|Boolean|Especifica se as políticas padrão de ambiente de educação do PC compartilhado devem ser desabilitadas. Para o Windows 10 RS2 e posterior, essa política será aplicada sem configurar Enabled como true.|
|setPowerPolicies|[habilitação] (.. /Resources/Intune-Shared-Enablement
.MD)|Especifica se as políticas de energia do PC compartilhada padrão devem ser ativado/desativado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disablePowerPolicies|Boolean|Especifica se as políticas padrão de energia do PC compartilhado devem ser desabilitadas.|
|signInOnResume|[habilitação] (.. /Resources/Intune-Shared-Enablement
.MD)|Especifica o requisito para entrar no sempre que o dispositivo retorna do modo de suspensão. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|disableSignInOnResume|Boolean|Desabilita o requisito de entrar sempre que o dispositivo sai do modo de suspensão.|
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
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
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




