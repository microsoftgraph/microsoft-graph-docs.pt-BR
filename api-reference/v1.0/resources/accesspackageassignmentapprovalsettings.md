---
title: tipo complexo accessPackageAssignmentApprovalSettings
description: Especifica as configurações para aprovação de uma solicitação para uma atribuição de pacote de acesso em uma política de atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5109cdd2482c43188409f891f782179bc1a39ebb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608261"
---
# <a name="accesspackageassignmentapprovalsettings-complex-type"></a>tipo complexo accessPackageAssignmentApprovalSettings

Namespace: microsoft.graph

Usado para a **propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso](accesspackageassignmentpolicy.md). Fornece configurações adicionais para indicar se a aprovação é necessária para novas solicitações para uma atribuição de pacote de acesso por meio dessa política ou para atualizações para solicitações existentes e para selecionar quem deve aprovar cada solicitação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isApprovalRequiredForAdd|Booliano|Se `false,` , em seguida, a aprovação não for necessária para novas solicitações nesta política.|
|isApprovalRequiredForUpdate|Booliano|If `false`, then approval is not required for updates to requests in this policy.|
|Estágios|[Coleção accessPackageApprovalStage](../resources/accesspackageapprovalstage.md)|Se a aprovação for necessária, os elementos um, dois ou três desta coleção definem cada uma das etapas de aprovação. Uma matriz vazia estará presente se nenhuma aprovação for necessária.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentApprovalSettings",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "stages": [
    {
      "@odata.type": "microsoft.graph.accessPackageApprovalStage"
    }
  ]
}
```


