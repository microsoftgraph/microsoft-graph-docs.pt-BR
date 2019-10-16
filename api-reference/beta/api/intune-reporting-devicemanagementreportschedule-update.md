---
title: Atualizar deviceManagementReportSchedule
description: Atualiza as propriedades de um objeto deviceManagementReportSchedule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f46c8881e1b936f224bd6a4f5c493f0fd69bb997
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537167"
---
# <a name="update-devicemanagementreportschedule"></a>Atualizar deviceManagementReportSchedule

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration. ReadWrite. All, DeviceManagementApps. ReadWrite. All, DeviceManagementManagedDevices. ReadWrite. All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para esta entidade|
|reportScheduleName|Cadeia de caracteres|Nome da agenda|
|subject|String|Assunto dos relatórios agendados que são entregues|
|email|String collection|Emails para os quais os relatórios agendados são entregues|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Frequência da entrega de relatórios agendados. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Hora de início da entrega dos relatórios agendados|
|endDateTime|DateTimeOffset|Hora em que a entrega dos relatórios agendados termina|
|userId|Cadeia de caracteres|A ID do usuário que criou o relatório|
|reportName|Cadeia de caracteres|Nome do relatório|
|filter|Cadeia de caracteres|Filtros aplicados no relatório|
|select|String collection|Colunas selecionadas do relatório|
|Classificadoporativado|String collection|Ordenação de colunas no relatório|
|formato|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório agendado. Os valores possíveis são: `csv` e `pdf`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-type: application/json
Content-length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "00bb9785-9785-00bb-8597-bb008597bb00",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```






