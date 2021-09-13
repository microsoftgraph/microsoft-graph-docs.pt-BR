---
title: Criar deviceManagementExportJob
description: Crie um novo objeto deviceManagementExportJob.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 39d3f8e2ad3b37a8311917328931d7f501d6baae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59099515"
---
# <a name="create-devicemanagementexportjob"></a>Criar deviceManagementExportJob

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementExportJob.

A tabela a seguir mostra as propriedades necessárias ao criar deviceManagementExportJob.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo dessa entidade|
|reportName|String|Nome do relatório|
|filter|Cadeia de caracteres|Filtros aplicados no relatório|
|select|Coleção String|Colunas selecionadas no relatório|
|formato|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório exportado. Os valores possíveis são: `csv` e `pdf`.|
|snapshotId|Cadeia de caracteres|Um instantâneo é um subconjunto identificável do conjuntos de dados representado pelo ReportName. Uma id sessionId ou CachedReportConfiguration pode ser usada aqui. Se uma sessionId for especificada, Filter, Select e OrderBy serão aplicados aos dados representados pela sessionId. Filter, Select e OrderBy não podem ser especificados juntamente com uma id CachedReportConfiguration.|
|localizationType|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Configura como o trabalho de exportação solicitado é localizado. Os valores possíveis são: `localizedValuesAsAdditionalColumn` e `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Status do trabalho de exportação. Os valores possíveis são: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|Cadeia de caracteres|Local temporário do relatório exportado|
|requestDateTime|DateTimeOffset|Hora em que o relatório exportado foi solicitado|
|expirationDateTime|DateTimeOffset|Tempo em que o relatório exportado expira|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




