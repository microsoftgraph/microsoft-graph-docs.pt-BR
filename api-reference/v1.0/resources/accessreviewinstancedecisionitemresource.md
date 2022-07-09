---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Representa o recurso associado ao item de decisão.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 10a85d2d2a25e5497204e9f517253e602298dd02
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697754"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemResource

Namespace: microsoft.graph

Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. O recurso é identificado por um objeto accessReviewInstanceDecisionItemResource. 

[accessReviewInstanceDecisionItemResource](accessreviewinstancedecisionitemresource.md) é um tipo aberto que permite que outras propriedades sejam passadas e é o tipo base para os seguintes recursos: [accessReviewInstanceDecisionItemAccessPackageAssignmentPolicyResource](accessreviewinstancedecisionitemaccesspackageassignmentpolicyresource.md), [accessReviewInstanceDecisionItemAzureRoleResource](accessreviewinstancedecisionitemazureroleresource.md) e [accessReviewInstanceDecisionItemServicePrincipalResource](accessreviewinstancedecisionitemserviceprincipalresource.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição do recurso|
|id|Cadeia de caracteres|Identificador do recurso|
|type|Cadeia de caracteres|Tipo de recurso. Os tipos incluem: `Group`, `ServicePrincipal`, `DirectoryRole`, `AzureRole`, `AccessPackageAssignmentPolicy`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
