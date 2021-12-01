---
title: Tipo de recurso accessPackageAssignmentRequestRequirements
description: Identifica os requisitos necessários para solicitar o pacote de acesso especificado.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96179dd106936d5f39d5636231788ad51837473e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242183"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>Tipo de recurso accessPackageAssignmentRequestRequirements

Namespace: microsoft.graph

Representa os requisitos que um chamador deve atender para criar com êxito **um accessPackageAssignmentRequest** para **o accessPackage** especificado como parte da URL. Os requisitos são determinados pela avaliação de políticas associadas ao **accessPackage**. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Booliano|Indica se o solicitante tem permissão para definir uma agenda personalizada.|
|isApprovalRequiredForAdd|Booliano|Indica se uma solicitação para adicionar deve ser aprovada por um aprovador.|
|isApprovalRequiredForUpdate|Booliano|Indica se uma solicitação de atualização deve ser aprovada por um aprovador.|
|policyDescription|Cadeia de Caracteres|A descrição da política que o usuário está tentando solicitar acesso usando.|
|policyDisplayName|Cadeia de Caracteres|O nome de exibição da política que o usuário está tentando solicitar acesso usando.|
|policyId|Cadeia de Caracteres|O identificador da política à que esses requisitos estão associados. Esse identificador pode ser usado ao criar uma nova solicitação de atribuição.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Restrições de agendamento impostas, se alguma.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


