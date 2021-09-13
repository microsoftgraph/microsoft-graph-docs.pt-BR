---
title: Tipo de recurso defaultDeviceCompliancePolicy
description: Regras de política de conformidade de dispositivo padrão que são aplicadas em toda a conta.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcaf6a82113106c369f0fa2c1b3715d9801aa348
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033753"
---
# <a name="defaultdevicecompliancepolicy-resource-type"></a>Tipo de recurso defaultDeviceCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Regras de política de conformidade de dispositivo padrão que são aplicadas em toda a conta.


Herda de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar defaultDeviceCompliancePolicies](../api/intune-deviceconfig-defaultdevicecompliancepolicy-list.md)|[Coleção defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|Listar propriedades e relações dos [objetos defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|
|[Obter defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-get.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|Leia propriedades e relações do [objeto defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|
|[Criar defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-create.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|Crie um novo [objeto defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|
|[Excluir defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-delete.md)|Nenhum|Exclui um [defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md).|
|[Atualizar defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-update.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|Atualize as propriedades de [um objeto defaultDeviceCompliancePolicy.](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)|A lista de ações agendadas por regra para essa política de conformidade. Essa é uma propriedade necessária ao criar qualquer política de conformidade individual por plataforma. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultDeviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



