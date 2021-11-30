---
title: Tipo de recurso accessReviewInstanceDecisionItemResource
description: Representa o recurso associado ao item de decisão.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b9b411d1b101d1f2fdc746d2bfb70d0dae8ede9b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226551"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemResource

Namespace: microsoft.graph

Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso identificado por um objeto accessReviewInstanceDecisionItemResource. accessReviewInstanceDecisionItemResource é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome de exibição do recurso|
|id|String|Identificador do recurso|
|type|String|Tipo de recurso. Os tipos `Group` incluem: `ServicePrincipal` , , , , `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .|

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
