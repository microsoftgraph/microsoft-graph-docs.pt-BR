---
title: Tipo de recurso archivedPrintJob
description: Um registro de um trabalho de impressão de "estado final" (concluído, anulado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 90e694b0a6bd4019fd75f871b03bcc34d999df3a
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971382"
---
# <a name="archivedprintjob-resource-type"></a>Tipo de recurso archivedPrintJob

Namespace: microsoft.graph

Um registro de um trabalho de impressão de "estado final" (concluído, anulado ou com falha) usado para fins de relatório. Este não é um trabalho de impressão ativo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O GUID do trabalho de impressão arquivado. Somente leitura.|
|printerId|Cadeia de caracteres|A ID da impressora para a qual o trabalho foi enfileirado. Somente leitura.|
|processingState|printJobProcessingState|O estado de processamento final do trabalho de impressão. Somente leitura.|
|createdDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi criado. Somente leitura.|
|acquiredDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi adquirido pela impressora, se houver. Somente leitura.|
|completionDateTime|DateTimeOffset|O dateTimeOffset quando o trabalho foi concluído, cancelado ou anulado. Somente leitura.|
|acquiredByPrinter|Booleano|True se o trabalho foi adquirido por uma impressora; caso contrário, false. Somente leitura.|
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
