---
title: Tipo de recurso deviceManagementReports
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f05d668ad7397236868f023f76191e46a77e522
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730970"
---
# <a name="devicemanagementreports-resource-type"></a>Tipo de recurso deviceManagementReports

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceManagementReports](../api/intune-reporting-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Ler propriedades e relações do [objeto deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .|
|[Atualizar deviceManagementReports](../api/intune-reporting-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|Atualize as propriedades de [um objeto deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) .|
|[Ação getDeviceNonComplianceReport](../api/intune-reporting-devicemanagementreports-getdevicenoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getNoncompliantDevicesAndSettingsReport](../api/intune-reporting-devicemanagementreports-getnoncompliantdevicesandsettingsreport.md)|Fluxo|Ainda não documentado|
|[Ação getPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getPolicyNonComplianceMetadata](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancemetadata.md)|Fluxo|Ainda não documentado|
|[Ação getPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getpolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[Ação getSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getsettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getReportFilters](../api/intune-reporting-devicemanagementreports-getreportfilters.md)|Fluxo|Ainda não documentado|
|[Ação getHistoricalReport](../api/intune-reporting-devicemanagementreports-gethistoricalreport.md)|Fluxo|Ainda não documentado|
|[Ação getConfigurationPolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[Ação getConfigurationPolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationpolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getConfigurationSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getconfigurationsettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getDeviceManagementIntentSettingsReport](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentsettingsreport.md)|Fluxo|Ainda não documentado|
|[Ação getDeviceManagementIntentPerSettingContributingProfiles](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentpersettingcontributingprofiles.md)|Fluxo|Ainda não documentado|
|[Ação getCompliancePolicyNonComplianceSummaryReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancesummaryreport.md)|Fluxo|Ainda não documentado|
|[Ação getCompliancePolicyNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancepolicynoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getComplianceSettingNonComplianceReport](../api/intune-reporting-devicemanagementreports-getcompliancesettingnoncompliancereport.md)|Fluxo|Ainda não documentado|
|[Ação getCachedReport](../api/intune-reporting-devicemanagementreports-getcachedreport.md)|Fluxo|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para esta entidade|

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





