---
title: Tipo de recurso deviceManagementReports
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de relatórios.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 531d1a7e3f2529982f5c1da4ab908edc765b7dc6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039347"
---
# <a name="devicemanagementreports-resource-type"></a>Tipo de recurso deviceManagementReports

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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
|[ação getDeviceManagementIntentPerSettingContributingProfiles](../api/intune-reporting-devicemanagementreports-getdevicemanagementintentpersettingcontributingprofiles.md)|Fluxo|Ainda não documentado|
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
|cachedReportConfigurations|[Coleção deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Entidade que representa a configuração de um relatório em cache|
|exportJobs|[Coleção deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)|Entidade que representa um trabalho para exportar um relatório|
|reportSchedules|[Coleção deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md)|Entidade que representa um cronograma para o qual os relatórios são entregues|

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



