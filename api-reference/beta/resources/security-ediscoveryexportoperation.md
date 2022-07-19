---
title: Tipo de recurso ediscoveryExportOperation
description: Representa o processo de uma exportação de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 14a4d85e2efada576b3e0d8ff9bc0a1bdfe64cf6
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838623"
---
# <a name="ediscoveryexportoperation-resource-type"></a>Tipo de recurso ediscoveryExportOperation

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de uma exportação de Descoberta Eletrônica.

Herda de [caseOperation](../resources/security-caseoperation.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[getDownloadUrl](../api/security-ediscoveryexportoperation-getdownloadurl.md)|String| Retorna a URL para a exportação.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.security.caseAction](../resources/security-caseoperation.md#caseaction-values)| O tipo de ação que a operação representa. Os valores possíveis são: `addToReviewSet`,`applyTags`,`contentExport`,,`convertToPdf`,`estimateStatistics``purgeData`|
|azureBlobContainer|String| O nome do local de armazenamento do Azure em que a exportação será armazenada. Isso se aplica somente às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|azureBlobToken|String| O token SAS para o local de armazenamento do Azure.  Isso se aplica somente às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|completedDateTime|DateTimeOffset| A data e a hora em que a exportação foi concluída.|
|createdBy|[identitySet](../resources/identityset.md)| O usuário que iniciou a operação de exportação.|
|createdDateTime|DateTimeOffset| A data e a hora em que a exportação foi criada.|
|descrição|String| A descrição fornecida para a exportação.|
|Exportoptions|microsoft.graph.security.exportOptions| As opções fornecidas para a exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/security-ediscoveryreviewset-export.md). Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.security.exportFileStructure|As opções fornecidas que especificam a estrutura da exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/security-ediscoveryreviewset-export.md). Os valores possíveis são: `none`, `directory`, `pst`.|
|id|String| A ID da operação. Somente leitura. |
|outputName|String| O nome fornecido para a exportação.|
|percentProgress|Int32| O progresso da operação.|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultado específicas de êxito e falha. Herdado de [caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.security.caseOperationStatus](../resources/security-caseoperation.md#caseoperationstatus-values)| O status da operação de caso. Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="exportoptions-values"></a>Valores de exportOptions

|Member|Descrição|
|:----|-----------|
|originalFiles|Inclua arquivos originais em formato nativo. Por exemplo: docx, xlsx, pptx, doc, xlst, pptm etc.|
|texto|Inclua texto extraído dos arquivos originais.|
|pdfReplacement|Substitua o arquivo original pela versão em PDF quando disponível.|
|Fileinfo|Inclua metadados de arquivos originais em um arquivo de carregamento.|
|tags|Inclua informações de marca em fileInfo.|

### <a name="exportfilestructure-values"></a>Valores exportFileStructure

|Member|Descrição|
|:----|-----------|
|Nenhum|Estrutura de arquivo padrão.|
|Diretório|Todos os arquivos em uma pasta singe chamada NativeFiles.|
|Pst|Os emails serão agrupados no formato pst.|

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

