---
title: Tipo de recurso ediscoveryExportOperation
description: Representa o processo de uma exportação de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 499f019fa9933522b91d9d0f1aeff518e43ff13b
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945052"
---
# <a name="ediscoveryexportoperation-resource-type"></a>Tipo de recurso ediscoveryExportOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de uma exportação de Descoberta Eletrônica.

Herda de [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[getDownloadUrl](../api/security-ediscoveryexportoperation-getdownloadurl.md)|Cadeia de caracteres| Retorna a URL para a exportação.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|azureBlobContainer|Cadeia de caracteres| O nome do local de armazenamento do Azure em que a exportação será armazenada. Isso se aplica somente às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|azureBlobToken|Cadeia de caracteres| O token SAS para o local de armazenamento do Azure.  Isso se aplica somente às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|completedDateTime|DateTimeOffset| A data e a hora em que a exportação foi concluída.|
|createdBy|[identitySet](../resources/identityset.md)| O usuário que iniciou a operação de exportação.|
|createdDateTime|DateTimeOffset| A data e a hora em que a exportação foi criada.|
|descrição|Cadeia de caracteres| A descrição fornecida para a exportação.|
|Exportoptions|microsoft.graph.ediscovery.exportOptions| As opções fornecidas para a exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/security-ediscoveryreviewset-export.md). Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|As opções fornecidas que especificam a estrutura da exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/security-ediscoveryreviewset-export.md). Os valores possíveis são: `none`, `directory`, `pst`.|
|id|Cadeia de caracteres| A ID da operação. Somente leitura. |
|outputName|Cadeia de caracteres| O nome fornecido para a exportação.|
|percentProgress|Int32| O progresso da operação.|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultado específicas de êxito e falha. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|reviewSet|[microsoft.graph.security.ediscoveryReviewSet](../resources/security-ediscoveryreviewset.md)|    Examine o conjunto de onde os documentos são exportados.|
|reviewSetQuery|[microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md)|A consulta do conjunto de revisão que é usada para filtrar os documentos para exportação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryExportOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```

