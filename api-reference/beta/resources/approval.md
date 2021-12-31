---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um accessPackageAssignmentRequest ou userConsentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ccc04245cb3637290d75d842be88b55d84e832a3
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651516"
---
# <a name="approval-resource-type"></a>tipo de recurso de aprovação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), o objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` . Uma única solicitação de etapa pode ter uma etapa associada a ela na qual os aprovadores podem agir. Da mesma forma, uma solicitação em várias etapas pode ter várias etapas associadas a ela nas quais os aprovadores podem agir. No entanto, em aprovações em várias etapas, as etapas pendentes e concluídas anteriormente são mostradas.

Em [userConsentRequests](../resources/userconsentrequest.md), o objeto de aprovação para decisões associadas a uma solicitação.

Em [Gerenciamento de função](../resources/rolemanagement.md), as decisões de aprovar ou negar atribuições de função.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Obter aprovação](../api/approval-get.md) | [aprovação](approval.md) | Recupere as propriedades de um **objeto de aprovação.** |


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador do objeto de aprovação.  No gerenciamento de direitos, ele é o mesmo identificador do identificador da solicitação de atribuição [do pacote de acesso.](accesspackageassignmentrequest.md)|
|etapas|[Coleção approvalStep](../resources/approvalstep.md)|Usado para representar a decisão associada a uma única etapa no processo de aprovação configurado em [approvalStage](../resources/approvalstage.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Estágios|[coleção approvalStage](../resources/approvalstage.md)|Usada para a **propriedade approvalStages** das configurações de aprovação **na propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "baseType": "microsoft.graph.entity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
