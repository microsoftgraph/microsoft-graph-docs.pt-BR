---
title: Tipo de recurso deviceManagementExportJob
description: Entidade que representa um trabalho para exportar um relatório
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de9cf79f34b3f1d6c69ff3fb3d4018995b01c577
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730305"
---
# <a name="devicemanagementexportjob-resource-type"></a>Tipo de recurso deviceManagementExportJob

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um trabalho para exportar um relatório

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|[Coleção deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Listar propriedades e relações dos [objetos deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Obter deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Ler propriedades e relações do objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Criar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Crie um novo [objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Excluir deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|Nenhum|Exclui um [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Atualizar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Atualize as propriedades de [um objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para esta entidade|
|Reportname|String|Nome do relatório|
|filter|String|Filtros aplicados no relatório|
|select|Conjunto de cadeias de caracteres|Colunas selecionadas no relatório|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório exportado. Os valores possíveis são: `csv` e `pdf`.|
|snapshotId|String|Um instantâneo é um subconjunto identificável do conjunto de dados representado pelo ReportName. Uma id sessionId ou CachedReportConfiguration pode ser usada aqui. Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId. Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.|
|localizationType|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Configura como o trabalho de exportação solicitado é localizado. Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Status do trabalho de exportação. Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|Cadeia de caracteres|Local temporário do relatório exportado|
|requestDateTime|DateTimeOffset|Hora em que o relatório exportado foi solicitado|
|expirationDateTime|DateTimeOffset|Hora em que o relatório exportado expira|

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





