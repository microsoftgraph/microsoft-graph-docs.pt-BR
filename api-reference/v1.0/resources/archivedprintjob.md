---
title: Tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516922"
---
# <a name="archivedprintjob-resource-type"></a>Tipo de recurso archivedPrintJob

Namespace: microsoft.graph

Um registro de um trabalho de impressão "estado final" (concluído, abortado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|GUID do trabalho de impressão arquivado. Somente leitura.|
|printerId|Cadeia de caracteres|A ID da impressora na fila do trabalho. Somente leitura.|
|processingState|printJobProcessingState|O estado final de processamento do trabalho de impressão. Somente leitura.|
|createdDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi criado. Somente leitura.|
|acquiredDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi adquirido pela impressora, se for o caso. Somente leitura.|
|completionDateTime|DateTimeOffset|DateTimeOffset quando o trabalho foi concluído, cancelado ou abortado. Somente leitura.|
|acquiredByPrinter|Booliano|True se o trabalho foi adquirido por uma impressora; false caso contrário. Somente leitura.|
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