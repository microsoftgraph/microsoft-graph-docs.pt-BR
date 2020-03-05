---
title: tipo de recurso deviceManagementExportJob
description: Entidade que representa um trabalho para exportar um relatório
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60977b341516fcd7fb331a49d188a6842a44b0cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523804"
---
# <a name="devicemanagementexportjob-resource-type"></a>tipo de recurso deviceManagementExportJob

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um trabalho para exportar um relatório

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementExportJobs](../api/intune-reporting-devicemanagementexportjob-list.md)|coleção [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Listar Propriedades e relações dos objetos [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Obter deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-get.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Leia as propriedades e as relações do objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Criar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-create.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Criar um novo objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|
|[Excluir deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-delete.md)|Nenhum|Exclui [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).|
|[Atualizar deviceManagementExportJob](../api/intune-reporting-devicemanagementexportjob-update.md)|[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Atualiza as propriedades de um objeto [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para esta entidade|
|reportName|String|Nome do relatório|
|filter|String|Filtros aplicados no relatório|
|select|String collection|Colunas selecionadas do relatório|
|formato|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório exportado. Os valores possíveis são: `csv` e `pdf`.|
|instantâneoid|String|Um instantâneo é um subconjunto identificável do DataSet representado pelo ReportName. Uma ID de Identificação_da_sessão ou CachedReportConfiguration pode ser usada aqui. Se uma Identificação_da_sessão for especificada, Filter, Select e OrderBy serão aplicadas aos dados representados pela Identificação_da_sessão. Filter, Select e OrderBy não podem ser especificados junto com uma ID CachedReportConfiguration.|
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
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



