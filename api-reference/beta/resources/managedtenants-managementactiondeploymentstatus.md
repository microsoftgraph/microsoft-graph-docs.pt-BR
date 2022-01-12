---
title: tipo de recurso managementActionDeploymentStatus
description: Representa o status de implantação de um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2f9b8ce493239e4c33bc2f20c615897afab41d9b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791879"
---
# <a name="managementactiondeploymentstatus-resource-type"></a>tipo de recurso managementActionDeploymentStatus

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de implantação de um determinado locatário gerenciado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|managementActionId|String|O identificador da ação de gerenciamento. Obrigatório. Somente leitura.|
|managementTemplateId|String|O identificador de modelo de gerenciamento usado para gerar a ação de gerenciamento. Obrigatório. Somente leitura.|
|status|managementActionStatus|O status da ação de gerenciamento. Os valores possíveis são: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`. Obrigatório.|
|workloadActionDeploymentStatuses|[coleção microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md)|A coleção de estatuetas de implantação de ação de carga de trabalho para a ação de gerenciamento determinada. Opcional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
