---
title: Tipo de recurso sensitivityLabelAssignment
description: Fornece detalhes sobre um rótulo de confidencialidade atribuído a um arquivo SharePoint ou OneDrive for Business.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3f46f0c064bb03286f1d38ba9c915db243acff9f
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917798"
---
# <a name="sensitivitylabelassignment-resource-type"></a>Tipo de recurso sensitivityLabelAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece detalhes sobre um rótulo de confidencialidade atribuído a um [arquivo](./driveitem.md) SharePoint ou OneDrive for Business.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignmentMethod|sensitivityLabelAssignmentMethod|Indica se a atribuição de rótulo é feita automaticamente, como um padrão ou uma operação privilegiada. Os valores possíveis são: `standard`, `privileged`, `auto`, `unknownFutureValue`.|
|sensitivityLabelId|Cadeia de Caracteres|O identificador exclusivo do rótulo de confidencialidade atribuído ao arquivo.|
|tenantId|String|O identificador exclusivo do locatário que hospeda o arquivo quando esse rótulo é aplicado.|

### <a name="sensitivitylabelassignmentmethod-values"></a>Valores sensitivityLabelAssignmentMethod

| Member             | Descrição                                    |
|:------------------ |:-----------------------------------------------|
| Padrão           | O método de atribuição para o rótulo é padrão.|
| Privilegiada         | O método de atribuição para o rótulo é privilegiado. Indica que o rótulo é aplicado manualmente por um usuário ou por um administrador.|
| Automático               | Indica que o rótulo é aplicado automaticamente pelo sistema devido a uma política configurada, como rótulo padrão ou classificação automática de conteúdo confidencial.|
| unknownFutureValue | Valor de sentinel de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Rótulos|[extractSensitivityLabelsResult](./extractsensitivitylabelsresult.md)|Lista de rótulos de confidencialidade atribuídos a um arquivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitivityLabelAssignment",
  "assignmentMethod": "String",
  "sensitivityLabelId": "String",
  "tenantId": "String"
}
```

