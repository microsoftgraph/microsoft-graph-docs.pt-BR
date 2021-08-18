---
title: Tipo de recurso deviceManagementAutopilotPolicyStatusDetail
description: Item de detalhes do status da política contido por um evento de piloto automático.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3cacc18dae925f6c95333693b2bf928b1f466f28
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264350"
---
# <a name="devicemanagementautopilotpolicystatusdetail-resource-type"></a>Tipo de recurso deviceManagementAutopilotPolicyStatusDetail

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Item de detalhes do status da política contido por um evento de piloto automático.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementAutopilotPolicyStatusDetails](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-list.md)|[Coleção deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Listar propriedades e relações dos [objetos deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|
|[Obter deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Leia propriedades e relações do [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|
|[Criar deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-create.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Crie um novo [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|
|[Excluir deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-delete.md)|Nenhum|Exclui um [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).|
|[Atualizar deviceManagementAutopilotPolicyStatusDetail](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-update.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Atualize as propriedades de [um objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|displayName|Cadeia de caracteres|O nome amigável da política.|
|policyType|[deviceManagementAutopilotPolicyType](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|O tipo de política. Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|complianceStatus|[deviceManagementAutopilotPolicyComplianceStatus](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|O status de conformidade da política. Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|trackedOnEnrollmentStatus|Boolean|Indica se essa prolicy foi controlada como parte da sessão de sincronização de registro de inicialização de inicialização do piloto automático|
|lastReportedDateTime|DateTimeOffset|Timestamp do status da política relatada|
|errorCode|Int32|O errorode associado ao status de conformidade ou imposição da política. O código de erro para o status de imposição tem precedência se existir.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotPolicyStatusDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "String (identifier)",
  "displayName": "String",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```




