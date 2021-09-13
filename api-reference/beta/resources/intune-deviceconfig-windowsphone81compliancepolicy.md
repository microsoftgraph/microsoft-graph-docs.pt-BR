---
title: Tipo de recurso windowsPhone81CompliancePolicy
description: Essa classe contém as configurações de conformidade do Windows 8.1 Mobile.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac38562e2fd23ec8a772fad83a70b9578de434a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091591"
---
# <a name="windowsphone81compliancepolicy-resource-type"></a>Tipo de recurso windowsPhone81CompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa classe contém as configurações de conformidade do Windows 8.1 Mobile.


Herda de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsPhone81CompliancePolicies](../api/intune-deviceconfig-windowsphone81compliancepolicy-list.md)|Coleção [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Listar propriedades e relações dos objetos [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).|
|[Obter windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-get.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Ler propriedades e relações do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).|
|[Criar windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-create.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Cria um novo objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).|
|[Excluir windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-delete.md)|Nenhum|Excluir um [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).|
|[Atualizar windowsPhone81CompliancePolicy](../api/intune-deviceconfig-windowsphone81compliancepolicy-update.md)|[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md)|Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|passwordBlockSimple|Boolean|Se a sincronização do calendário deve ou não ser bloqueada.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha.|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 0 a 24|
|passwordRequired|Boolean|Se uma senha deve ou não ser exigida.|
|osMinimumVersion|String|Versão mínima do Windows Phone.|
|osMaximumVersion|String|Versão máxima do Windows Phone.|
|storageRequireEncryption|Booliano|Exige criptografia em dispositivos Windows Phone.|

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
  "@odata.type": "microsoft.graph.windowsPhone81CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequired": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "storageRequireEncryption": true
}
```



