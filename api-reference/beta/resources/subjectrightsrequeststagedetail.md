---
title: Tipo de recurso subjectRightsRequestStageDetail
description: Representa as propriedades dos estágios de uma solicitação de direitos de assunto
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2d4f62a704b115e9fb8a85525bb4cae818eb7a2
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60444706"
---
# <a name="subjectrightsrequeststagedetail-resource-type"></a>Tipo de recurso subjectRightsRequestStageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as propriedades dos estágios de uma solicitação de direitos de assunto. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|erro|[publicError](../resources/publicerror.md)|Descreve o erro, se for o caso, para o estágio atual.|
|stage|subjectRightsRequestStage|O estágio da solicitação de direitos de assunto. Os possíveis valores são: `contentRetrieval`, `contentReview`, `generateReport`, `contentDeletion`, `caseResolved`, `unknownFutureValue`.|
|status|subjectRightsRequestStageStatus|Status do estágio atual. Os valores possíveis são: `notStarted`, `current`, `completed`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestStageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestStageDetail",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "stage": "microsoft.graph.subjectRightsRequestStage",
  "status": "microsoft.graph.subjectRightsRequestStageStatus"
}
```

