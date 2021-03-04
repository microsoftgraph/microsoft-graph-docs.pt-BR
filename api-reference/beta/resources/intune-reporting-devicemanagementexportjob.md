---
title: Tipo de recurso deviceManagementExportJob
description: Entidade que representa um trabalho para exportar um relatório
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bef520a455a702e2f9f8c2a0926581b01e8d7418
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440189"
---
# <a name="devicemanagementexportjob-resource-type"></a>Tipo de recurso deviceManagementExportJob

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um trabalho para exportar um relatório

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[Coleção deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Listar propriedades e relações dos objetos [deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Obter deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Leia propriedades e relações do [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Criar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Crie um novo [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|
|[Excluir deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|Nenhum(a)|Exclui um [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Atualizar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Atualize as propriedades de [um objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo dessa entidade|
|reportName|String|Nome do relatório|
|filter|String|Filtros aplicados no relatório|
|select|Coleção de cadeias de caracteres|Colunas selecionadas no relatório|
|formato|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório exportado. Os valores possíveis são: `csv` e `pdf`.|
|snapshotId|String|Um instantâneo é um subconjunto identificável do conjuntos de dados representado pelo ReportName. Uma id sessionId ou CachedReportConfiguration pode ser usada aqui. Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId. Filter, Select e OrderBy não podem ser especificados juntamente com uma id CachedReportConfiguration.|
|localizationType|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Configura como o trabalho de exportação solicitado é localizado. Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Status do trabalho de exportação. Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|Cadeia de caracteres|Local temporário do relatório exportado|
|requestDateTime|DateTimeOffset|Hora em que o relatório exportado foi solicitado|
|expirationDateTime|DateTimeOffset|Tempo em que o relatório exportado expira|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExportJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "format": "String",
  "snapshotId": "String",
  "localizationType": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```




