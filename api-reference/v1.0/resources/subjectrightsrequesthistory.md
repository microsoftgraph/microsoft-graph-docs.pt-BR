---
title: tipo de recurso subjectRightsRequestHistory
description: Representa o histórico de uma solicitação de direitos de assunto.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d8a990990d5b3935ab54d9abb6a5e22453af6965
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457642"
---
# <a name="subjectrightsrequesthistory-resource-type"></a>tipo de recurso subjectRightsRequestHistory

Namespace: microsoft.graph

Representa o histórico de uma solicitação de direitos de assunto.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|changedBy|[identitySet](../resources/identityset.md)|Identidade do usuário que alterou a solicitação de direitos de assunto.|
|eventDateTime|DateTimeOffset|Dados e hora em que a entidade foi alterada.|
|stage|subjectRightsRequestStage|O estágio em que a entidade foi alterada. Os possíveis valores são: `contentRetrieval`, `contentReview`, `generateReport`, `contentDeletion`, `caseResolved`, `unknownFutureValue`.|
|stageStatus|subjectRightsRequestStageStatus|O status do estágio quando a entidade foi alterada. Os valores possíveis são: `notStarted`, `current`, `completed`, `failed`, `unknownFutureValue`.|
|type|Cadeia de caracteres|Tipo de histórico.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectRightsRequestHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectRightsRequestHistory",
    "type": "String",
    "stage": "String",
    "stageStatus": "String",
    "eventDateTime": "String (timeStamp)",
    "changedBy": {
        "user": {
            "id": "String",
            "displayName": "String"
        }
    }
}
```

