---
title: Tipo de recurso managedTenant
description: Represente as operações disponíveis que interagem com a plataforma de gerenciamento de vários locatários.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9047977dd701e9844ae7158b6a6c1845a189de4e
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791900"
---
# <a name="managedtenant-resource-type"></a>Tipo de recurso managedTenant

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Como o recurso raiz da API Microsoft 365 Lighthouse, **managedTenant** representa os recursos disponíveis para um MSP (Provedor de Serviços Gerenciados) para dimensionar o gerenciamento remoto de seus locatários de clientes para ajudá-los a obter um estado íntegre e seguro.

A Microsoft 365 Lighthouse api é definida no subnamespace OData, `microsoft.graph.managedTenants` .

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aggregatedPolicyCompliances|[coleção microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Visão agregada das políticas de conformidade do dispositivo entre locatários gerenciados.|
|cloudPcConnections|[coleção microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|A coleção de conexões de computador na nuvem entre locatários gerenciados.|
|cloudPcDevices|[coleção microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|A coleção de dispositivos de computador na nuvem em locatários gerenciados.|
|cloudPcsOverview|[coleção microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Visão geral das informações do computador na nuvem em locatários gerenciados.|
|conditionalAccessPolicyCoverages|[coleção microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Visão agregada da cobertura da política de acesso condicional entre locatários gerenciados.|
|credentialUserRegistrationsSummaries|[coleção microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Informações de resumo para o registro do usuário para autenticação multifafa e redefinição de senha de autoatendido entre locatários gerenciados.|
|deviceCompliancePolicySettingStateSummaries|[coleção microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Informações de resumo para estados de configuração de política de conformidade de dispositivo entre locatários gerenciados.|
|managedDeviceCompliances|[coleção microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|A coleção de conformidade para dispositivos gerenciados em locatários gerenciados.|
|managedDeviceComplianceTrends|[Coleção microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Ideias de tendência para a conformidade do dispositivo entre locatários gerenciados.|
|managementActions|[Coleção microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|A coleção de ações de gerenciamento de linha de base entre locatários gerenciados.|
|managementActionTenantDeploymentStatuses|[coleção microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|O status de nível de locatário das ações de gerenciamento em locatários gerenciados.|
|managementIntents|[coleção microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|A coleção de intenções de gerenciamento de linha de base entre locatários gerenciados.|
|managementTemplates|[coleção microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|A coleção de modelos de gerenciamento de linha de base entre locatários gerenciados.|
|tenantGroups|[coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|A coleção de um grupo lógico de locatários gerenciados usados pela plataforma de gerenciamento de vários locatários.|
|locatários|[coleção microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|A coleção de locatários associados à entidade de gerenciamento.|
|tenantsCustomizedInformation|[coleção microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|A coleção de informações personalizadas em nível de locatário entre locatários gerenciados.|
|tenantsDetailedInformation|[coleção microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|O nível de locatário de coleção informações detalhadas entre locatários gerenciados.|
|tenantTags|[coleção microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|A coleção de marcas de locatários entre locatários gerenciados.|
|windowsDeviceMalwareStates|[coleção microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md)|O estado de malware para Windows dispositivos, registrados com Microsoft Endpoint Manager, em locatários gerenciados.|
|windowsProtectionStates|[coleção microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|O estado de proteção para Windows, registrado com Microsoft Endpoint Manager, entre locatários gerenciados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedTenant",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenant",
  "id": "String (identifier)"
}
```
