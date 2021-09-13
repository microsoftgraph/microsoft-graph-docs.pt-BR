---
title: Tipo de recurso deviceManagementReportSchedule
description: Entidade que representa um cronograma para o qual os relatórios são entregues
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f0a75f233880345d72e5d7dedcee033d8e1097d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039326"
---
# <a name="devicemanagementreportschedule-resource-type"></a>Tipo de recurso deviceManagementReportSchedule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa um cronograma para o qual os relatórios são entregues

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementReportSchedules](../api/intune-reporting-devicemanagementreportschedule-list.md)|[Coleção deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Listar propriedades e relações dos [objetos deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Obter deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-get.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Leia propriedades e relações do [objeto deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Criar deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-create.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Crie um novo [objeto deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|
|[Excluir deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-delete.md)|Nenhum|Exclui um [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).|
|[Atualizar deviceManagementReportSchedule](../api/intune-reporting-devicemanagementreportschedule-update.md)|[deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Atualize as propriedades de [um objeto deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo dessa entidade|
|reportScheduleName|Cadeia de Caracteres|Nome da agenda|
|assunto|Cadeia de caracteres|Assunto dos relatórios agendados que são entregues|
|emails|String collection|Emails para os quais os relatórios agendados são entregues|
|recurrence|[deviceManagementScheduledReportRecurrence](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|Frequência de entrega de relatório agendada. Os valores possíveis são: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|Hora em que a entrega dos relatórios agendados é iniciada|
|endDateTime|DateTimeOffset|Hora em que a entrega dos relatórios agendados termina|
|userId|Cadeia de caracteres|A ID do Usuário que criou o relatório|
|reportName|Cadeia de Caracteres|Nome do relatório|
|filter|Cadeia de Caracteres|Filtros aplicados no relatório|
|select|String collection|Colunas selecionadas no relatório|
|orderBy|String collection|Ordenação de colunas no relatório|
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



