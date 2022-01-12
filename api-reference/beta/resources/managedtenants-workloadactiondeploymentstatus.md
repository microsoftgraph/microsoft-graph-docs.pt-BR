---
title: Tipo de recurso workloadActionDeploymentStatus
description: Representa o status de implantação da ação de carga de trabalho.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 763ad6e70969565f15f9db159a423d6ec1bbb4a2
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792040"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a>Tipo de recurso workloadActionDeploymentStatus

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status de implantação da ação de carga de trabalho.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionId|String|O identificador exclusivo da ação de carga de trabalho. Obrigatório. Somente leitura.|
|deployedPolicyId|String|O identificador de qualquer política que foi criada aplicando a ação de carga de trabalho. Opcional. Somente leitura.|
|erro|[microsoft.graph.genericError](../resources/genericerror.md)|As informações detalhadas para exceções que ocorrem ao implantar a ação de carga de trabalho. Opcional. Obrigatório.|
|lastDeploymentDateTime|DateTimeOffset|A data e a hora em que a ação de carga de trabalho foi implantada pela última vez. Opcional.|
|status|workloadActionStatus|O status da implantação da ação de carga de trabalho. Os possíveis valores são: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
