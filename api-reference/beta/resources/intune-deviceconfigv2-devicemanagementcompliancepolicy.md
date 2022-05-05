---
title: Tipo de recurso deviceManagementCompliancePolicy
description: Gerenciamento de Dispositivos de Conformidade do Gerenciamento de Dispositivos
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c89d202aafea0d5245dcc33d88836f09a68eabe4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208775"
---
# <a name="devicemanagementcompliancepolicy-resource-type"></a>Tipo de recurso deviceManagementCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Gerenciamento de Dispositivos de Conformidade do Gerenciamento de Dispositivos

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementCompliancePolicies](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-list.md)|[Coleção deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Listar propriedades e relações dos [objetos deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Obter deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-get.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Leia as propriedades e as relações do [objeto deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Criar deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-create.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Crie um novo [objeto deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[Excluir deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-delete.md)|Nenhuma|Exclui um [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md).|
|[Atualizar deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-update.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|Atualize as propriedades de [um objeto deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) .|
|[atribuir ação](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-assign.md)|[Coleção deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Ainda não documentado|
|[Ação setScheduledActions](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-setscheduledactions.md)|[Coleção deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do documento de política. Gerado automaticamente.|
|nome|Cadeia de caracteres|Nome da política|
|descrição|Cadeia de caracteres|Descrição da política|
|Plataformas|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Plataformas para essa política. Os valores possíveis são: `none`, `android`, `iOS`, `macOS`, `windows10X`, `windows10`, `linux`, `unknownFutureValue`.|
|Tecnologias|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Tecnologias para essa política. Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`, `appleRemoteManagement`, `microsoftSense`, `exchangeOnline`, `linuxMdm`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|Data e hora de criação da política. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação da política. Essa propriedade é somente leitura.|
|settingCount|Int32|Número de configurações. Essa propriedade é somente leitura.|
|creationSource|Cadeia de Caracteres|Origem de criação de política|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|
|isAssigned|Boolean|Status da atribuição de política. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settings|[Coleção deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Configurações de política|
|assignments|[Coleção deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Atribuições de política|
|scheduledActionsForRule|[Coleção deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|A lista de ações agendadas para essa regra|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCompliancePolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true
}
```




