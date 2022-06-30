---
title: Tipo de recurso dispositionReviewStage
description: Representa um processo de revisão de vários níveis em que os revisores indicam em cada estágio da disposição se devem excluir ou manter ainda mais o item de conteúdo..
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: cc89d8c907fcd6ec84c4810f30e19921e6312d1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447521"
---
# <a name="dispositionreviewstage-resource-type"></a>Tipo de recurso dispositionReviewStage

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um processo de revisão de vários níveis em que os revisores indicam em cada estágio da disposição se devem excluir ou manter ainda mais o item de conteúdo.
Para obter detalhes, consulte [Disposição do conteúdo](/microsoft-365/compliance/disposition).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Crie um novo [objeto retentionLabel](../resources/security-retentionlabel.md) . |
|[Atualizar retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Atualize [o objeto retentionLabel](../resources/security-retentionlabel.md) . |


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva para cada estágio. |
|nome|Cadeia de caracteres|Nome que representa cada estágio em uma coleção. |
|reviewersEmailAddresses|Coleção de cadeias de caracteres|Uma coleção de revisores em cada estágio. |
|stageNumber|Int32|O número de sequência para cada estágio da revisão de disposição. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dispositionReviewStage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dispositionReviewStage",
  "id": "String (identifier)",
  "stageNumber": "Integer",
  "name": "String",
  "reviewersEmailAddresses": [
    "String"
  ]
}
```
