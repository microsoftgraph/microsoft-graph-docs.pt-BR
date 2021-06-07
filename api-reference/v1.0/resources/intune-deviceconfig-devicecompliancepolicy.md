---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8db918712004db04dae085aa607d5de6b82f180b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752137"
---
# <a name="devicecompliancepolicy-resource-type"></a>Tipo de recurso deviceCompliancePolicy

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. 

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCompliancePolicies](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|[Obter deviceCompliancePolicy](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|[ação assign](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Ainda não documentado|
|[ação scheduleActionsForRules](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|descrição|Cadeia de caracteres|Descrição fornecida pelo administrador da Configuração do dispositivo.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo.|
|versão|Int32|Versão da configuração do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|A lista de ações agendadas para essa regra|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus.|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus.|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para conformidade de dispositivos|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Visão geral de status de usuários para conformidade de dispositivos|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo do dispositivo para estado de configuração de conformidade|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




