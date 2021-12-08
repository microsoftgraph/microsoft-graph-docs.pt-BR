---
title: Tipo de recurso deviceManagementComplianceScheduledActionForRule
description: Ação agendada para a regra
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b5f5d652119f7a47e7543c82840d259174c3e59
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342801"
---
# <a name="devicemanagementcompliancescheduledactionforrule-resource-type"></a>Tipo de recurso deviceManagementComplianceScheduledActionForRule

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação agendada para a regra

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementComplianceScheduledActionForRules](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-list.md)|[Coleção deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Listar propriedades e relações dos [objetos deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Obter deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-get.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Leia propriedades e relações do [objeto deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Criar deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-create.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Crie um novo [objeto deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|
|[Excluir deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-delete.md)|Nenhum|Exclui um [deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md).|
|[Atualizar deviceManagementComplianceScheduledActionForRule](../api/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule-update.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|Atualize as propriedades de [um objeto deviceManagementComplianceScheduledActionForRule.](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave dessa configuração na política que a contém. Gerado automaticamente.|
|ruleName|Cadeia de caracteres|Nome da regra à qual essa ação agendada se aplica.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionConfigurations|[Coleção deviceManagementComplianceActionItem](../resources/intune-deviceconfigv2-devicemanagementcomplianceactionitem.md)|A lista de configurações de ações agendadas para essa política de conformidade. Essa coleção pode conter no máximo 100 elementos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplianceScheduledActionForRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplianceScheduledActionForRule",
  "id": "String (identifier)",
  "ruleName": "String"
}
```




