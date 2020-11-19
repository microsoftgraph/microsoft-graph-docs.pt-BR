---
title: tipo de recurso deviceManagementReportSchedule
description: Entidade que representa um cronograma para o qual os relatórios são entregues
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 121940d6bad85ed63589ae62254e667d7fd81c0e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307091"
---
# <a name="devicemanagementreportschedule-resource-type"></a>tipo de recurso deviceManagementReportSchedule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um cronograma para o qual os relatórios são entregues

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementReportSchedules](../api/intune-reporting-devicemanagementreportschedule-list.md)|coleção [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Listar Propriedades e relações dos objetos [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Obter deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Leia as propriedades e as relações do objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Criar deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Criar um novo objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .|
|[Excluir deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-delete.md)|Nenhum|Exclui [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).|
|[Atualizar deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Atualiza as propriedades de um objeto [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para esta entidade|
|reportScheduleName|String|Nome da agenda|
|assunto|String|Assunto dos relatórios agendados que são entregues|
|email|Coleção de cadeias de caracteres|Emails para os quais os relatórios agendados são entregues|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Frequência da entrega de relatórios agendados. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Hora de início da entrega dos relatórios agendados|
|endDateTime|DateTimeOffset|Hora em que a entrega dos relatórios agendados termina|
|userId|Cadeia de caracteres|A ID do usuário que criou o relatório|
|reportName|String|Nome do relatório|
|filter|String|Filtros aplicados no relatório|
|select|Coleção de cadeias de caracteres|Colunas selecionadas do relatório|
|Classificadoporativado|Coleção de cadeias de caracteres|Ordenação de colunas no relatório|
|formato|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Formato do relatório agendado. Os valores possíveis são: `csv`, `pdf`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReportSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "String (identifier)",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```




