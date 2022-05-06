---
author: FaithOmbongi
ms.localizationpriority: high
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: cc0f461ff3bbbd673c6ab83a1b71d5b836e37509
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247636"
---
<!-- markdownlint-disable MD041 -->

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  

| <!-- fake header--> | <!-- fake header--> |
|--|--|
|<ul> <li> [aggregatedPolicyCompliance](/graph/api/resources/managedTenants-aggregatedpolicycompliance) <li> [cloudPcConnection](/graph/api/resources/managedTenants-cloudpcconnection) <li> [cloudPcDevice](/graph/api/resources/managedTenants-cloudpcdevice) <li> [cloudPcOverview](/graph/api/resources/managedTenants-cloudpcoverview) <li> [conditionalAccessPolicyCoverage](/graph/api/resources/managedTenants-conditionalaccesspolicycoverage) <li> [credentialUserRegistrationsSummary](/graph/api/resources/managedTenants-credentialuserregistrationssummary) <li> [deviceCompliancePolicySettingStateSummary](/graph/api/resources/managedTenants-devicecompliancepolicysettingstatesummary) <li> [managedDeviceCompliance](/graph/api/resources/managedTenants-manageddevicecompliance) <li> [managedDeviceComplianceTrend](/graph/api/resources/managedTenants-manageddevicecompliancetrend) <li> [managedTenant](/graph/api/resources/managedTenants-managedtenant) <li> [managementAction](/graph/api/resources/managedTenants-managementaction) <li> [managementActionTenantDeploymentStatus](/graph/api/resources/managedTenants-managementactiontenantdeploymentstatus)  </ul>| <ul><li> [managementIntent](/graph/api/resources/managedTenants-managementintent) <li> [managementTemplate](/graph/api/resources/managedTenants-managementtemplate) <li> [riskyUser](/graph/api/resources/managedTenants-riskyuser) <li> [locatário](/graph/api/resources/managedTenants-tenant) <li> [tenantCustomizedInformation](/graph/api/resources/managedTenants-tenantcustomizedinformation) <li> [tenantDetailedInformation](/graph/api/resources/managedTenants-tenantdetailedinformation) <li> [tenantGroup](/graph/api/resources/managedTenants-tenantgroup) <li> [tenantRelationship](/graph/api/resources/tenantrelationship) <li> [tenantTag](/graph/api/resources/managedTenants-tenanttag) <li> [windowsDeviceMalwareState](/graph/api/resources/managedTenants-windowsdevicemalwarestate) <li> [windowsProtectionState](/graph/api/resources/managedTenants-windowsprotectionstate) </ul>|
