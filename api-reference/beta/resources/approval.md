---
title: tipo de recurso de aprovação
description: O objeto de aprovação associado a um accessPackageAssignmentRequest ou userConsentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 07990837a8774f512371fc5b09c400826321abd9
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454070"
---
# <a name="approval-resource-type"></a>tipo de recurso de aprovação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` . Uma única solicitação de etapa pode ter uma etapa associada a ela na qual os aprovadores podem agir. Da mesma forma, uma solicitação em várias etapas pode ter várias etapas associadas a ela nas quais os aprovadores podem agir. No entanto, em aprovações em várias etapas, as etapas pendentes e concluídas anteriormente são mostradas.

Em [userConsentRequests](../resources/userconsentrequest.md), o objeto de aprovação para decisões associadas a uma solicitação.

Em [Gerenciamento de função](../resources/rolemanagement.md), as decisões de aprovar ou negar atribuições de função.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Obter aprovação](../api/approval-get.md) | [aprovação](approval.md) | Recupere as propriedades de um **objeto de aprovação.** |


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador do objeto de aprovação.  No gerenciamento de direitos, ele é o mesmo identificador do identificador da solicitação de atribuição [do pacote de acesso.](accesspackageassignmentrequest.md)|
|etapas|[Coleção approvalStep](../resources/approvalstep.md)|Usado para representar a decisão associada a uma única etapa no processo de aprovação configurado em [approvalStage](../resources/approvalstage.md).|

## <a name="relationships"></a>Relacionamentos
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
