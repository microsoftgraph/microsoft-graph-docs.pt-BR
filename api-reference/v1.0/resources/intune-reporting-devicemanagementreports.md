---
title: Tipo de recurso deviceManagementReports
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e797beea7a282433dee07a39def45d2295a01adb796252b43522de863a8257b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246728"
---
# <a name="devicemanagementreports-resource-type"></a>Tipo de recurso deviceManagementReports

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Leia propriedades e relações do [objeto deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)|
|[Atualizar deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Atualize as propriedades de [um objeto deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)|
|[ação getDeviceNonComplianceReport](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getPolicyNonComplianceMetadata](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Fluxo|Ainda não documentado|
|[ação getPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[Ação getSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getReportFilters](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Fluxo|Ainda não documentado|
|[ação getHistoricalReport](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Fluxo|Ainda não documentado|
|[ação getConfigurationPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[ação getConfigurationPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getConfigurationSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationsettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getDeviceManagementIntentSettingsReport](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentsettingsreport.md)|Fluxo|Ainda não documentado|
|[ação getCompliancePolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[ação getCompliancePolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getComplianceSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancesettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[ação getCachedReport](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Fluxo|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo dessa entidade|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|exportJobs|[Coleção deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Entidade que representa um trabalho para exportar um relatório|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```




