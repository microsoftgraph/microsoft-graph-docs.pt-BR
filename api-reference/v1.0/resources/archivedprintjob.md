---
title: Tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9f6818801a12eb635a86350432108d3d0e3b6332
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109518"
---
# <a name="archivedprintjob-resource-type"></a>Tipo de recurso archivedPrintJob

Namespace: microsoft.graph

Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|GUID do trabalho de impressão arquivado. Somente leitura.|
|printerId|String|A ID da impressora na fila do trabalho. Somente leitura.|
|processingState|printJobProcessingState|O estado final de processamento do trabalho de impressão. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|acquiredDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi adquirido pela impressora, se for o caso. Somente leitura.|
|completionDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi concluído, cancelado ou abortado. Somente leitura.|
|acquiredByPrinter|Boolean|True se o trabalho foi adquirido por uma impressora; false caso contrário. Somente leitura.|
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
