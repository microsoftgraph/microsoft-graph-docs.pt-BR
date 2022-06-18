---
title: Tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão de "estado final" (concluído, anulado ou cancelado) usado para fins de relatório. Este não é um trabalho de impressão ativo."
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d6f9922dfbd50b347f38959a94f36520f425f2d9
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160605"
---
# <a name="archivedprintjob-resource-type"></a>Tipo de recurso archivedPrintJob

Namespace: microsoft.graph

Um registro de um trabalho de impressão de "estado final" (concluído, anulado ou cancelado) usado para fins de relatório. Este não é um trabalho de impressão ativo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O GUID do trabalho de impressão arquivado. Somente leitura.|
|printerId|Cadeia de Caracteres|A ID da impressora para a qual o trabalho foi enfileirado. Somente leitura.|
|processingState|printJobProcessingState|O estado de processamento final do trabalho de impressão. Somente leitura.|
|createdDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi criado. Somente leitura.|
|acquiredDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi adquirido pela impressora, se houver. Somente leitura.|
|completionDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi concluído, cancelado ou anulado. Somente leitura.|
|acquiredByPrinter|Boolean|True se o trabalho foi adquirido por uma impressora; caso contrário, false. Somente leitura.|
|copiesPrinted|Int32|O número de cópias que foram impressas. Somente leitura.|
|createdBy|[userIdentity](useridentity.md)|O usuário que criou o trabalho de impressão. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->
```json
    {   
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```
