---
title: Tipo de recurso caseExportOperation
description: Representa o processo de uma exportação de DescobertaSuporta.
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c3f69f459aec067608f350daddb5892b5e9ec06b
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793900"
---
# <a name="caseexportoperation-resource-type"></a>Tipo de recurso caseExportOperation

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o processo de uma exportação de DescobertaSuporta. O **caseExportOperation** só pode ser recuperado do header na resposta `Location` a uma exportação de conjuntos de [revisão.](../api/ediscovery-reviewset-export.md)

Herda de [caseOperation](../resources/ediscovery-caseoperation.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[getDownloadUrl](../api/ediscovery-caseexportoperation-getdownloadurl.md)|Cadeia de caracteres| Retorna a URL da exportação.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| A ação de caso dessa entidade sempre será `contentExport` . Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|azureBlobContainer|Cadeia de caracteres| O nome do local de armazenamento do Azure onde a exportação será armazenada. Isso só se aplica às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|azureBlobToken|Cadeia de caracteres| O token SAS para o local de armazenamento do Azure.  Isso só se aplica às exportações armazenadas em seu próprio local de armazenamento do Azure. |
|completedDateTime|DateTimeOffset| A data e a hora em que a exportação foi concluída.  Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|createdBy|[identitySet](../resources/identityset.md)| O usuário que iniciou a operação de exportação. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|createdDateTime|DateTimeOffset| A data e a hora em que a exportação foi criada. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|description|String| A descrição fornecida para a exportação. |
|exportOptions|microsoft.graph.ediscovery.exportOptions| As opções fornecidas para a exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/ediscovery-reviewset-export.md). Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|microsoft.graph.ediscovery.exportFileStructure|As opções fornecidas que especificam a estrutura da exportação. Para obter mais detalhes, consulte [reviewSet: export](../api/ediscovery-reviewset-export.md). Os valores possíveis são: `none`, `directory`, `pst`.|
|id|Cadeia de caracteres| A ID da operação. Somente leitura. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|outputName|String| O nome fornecido para a exportação.|
|percentProgress|Int32| O progresso da operação. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|resultInfo|[resultInfo](../resources/resultinfo.md)|Contém informações de resultados específicas de falha e sucesso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md).|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|O status da operação de caso. Herdado [de caseOperation](../resources/ediscovery-caseoperation.md). Os possíveis valores são: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

### <a name="exportoptions-values"></a>valores exportOptions

|Member| Descrição |
|:---|:---|
|originalFiles| Inclua cópias dos arquivos originais - exclua essa opção somente ao gerar relatórios. |
|texto| Inclua arquivos de texto extraídos brutos para cada documento. |
|pdfReplacement| Se os arquivos PDF redacted são gerados durante a revisão, esses arquivos estarão disponíveis para exportação. Você pode optar por exportar os PDFs redacted em vez dos arquivos nativos originais incluindo essa opção. |
|fileInfo| Inclua o arquivo de resumo e de carga - isso sempre deve ser incluído. |
|categorias| Inclua marcas de documento que foram aplicadas durante a revisão no arquivo de carga. |

### <a name="exportfilestructure-values"></a>valores exportFileStructure

|Member| Descrição |
|:---|:---|
|directory| Mapas à estrutura de diretório condensada comumente usada por ferramentas de Descoberta e. Todos os arquivos são exportados para um arquivo raiz chamado NativeFiles. |
|pst| Os emails são armazenados em PSTs enquanto documentos de sites são armazenados em pastas que representam a estrutura de pastas nativas original. |

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| O conjunto de revisão de onde o conteúdo está sendo exportado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
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
