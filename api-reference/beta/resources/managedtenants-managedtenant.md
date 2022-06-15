---
title: Tipo de recurso managedTenant
description: Representa as operações disponíveis que interagem com a plataforma de gerenciamento multilocatário.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4518a6b4f3b05e237e4a44c06bed12901369879b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094155"
---
# <a name="managedtenant-resource-type"></a>Tipo de recurso managedTenant

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Como o recurso raiz da API do Microsoft 365 Lighthouse, **managedTenant** representa os recursos disponíveis para um MSP (Provedor de Serviços Gerenciados) para dimensionar o gerenciamento remoto de seus locatários de clientes para ajudar a obtê-los em um estado íntegro e seguro.

A MICROSOFT 365 LIGHTHOUSE api é definida no subnamespace OData. `microsoft.graph.managedTenants`

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aggregatedPolicyCompliances|[Coleção microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Exibição agregada das políticas de conformidade do dispositivo entre locatários gerenciados.|
|auditEvents|[coleção microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|A coleção de eventos de auditoria entre locatários gerenciados.|
|cloudPcConnections|[Coleção microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|A coleção de conexões de PC na nuvem entre locatários gerenciados.|
|cloudPcDevices|[Coleção microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|A coleção de dispositivos de PC na nuvem entre locatários gerenciados.|
|cloudPcsOverview|[Coleção microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Visão geral das informações do PC na nuvem entre locatários gerenciados.|
|conditionalAccessPolicyCoverages|[coleção microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Exibição agregada da cobertura de política de acesso condicional entre locatários gerenciados.|
|credentialUserRegistrationsSummaries|[coleção microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Informações resumidas para registro de usuário para autenticação multifator e redefinição de senha de autoatendimento entre locatários gerenciados.|
|deviceCompliancePolicySettingStateSummaries|[coleção microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Informações resumidas para estados de configuração de política de conformidade do dispositivo entre locatários gerenciados.|
|managedDeviceCompliances|[Coleção microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|A coleção de conformidade para dispositivos gerenciados entre locatários gerenciados.|
|managedDeviceComplianceTrends|[Coleção microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Insights de tendência para conformidade do dispositivo entre locatários gerenciados.|
|managementActions|[Coleção microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|A coleção de ações de gerenciamento de linha de base entre locatários gerenciados.|
|managementActionTenantDeploymentStatuses|[coleção microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|O status de nível de locatário das ações de gerenciamento entre locatários gerenciados.|
|managementIntents|[Coleção microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|A coleção de intenções de gerenciamento de linha de base entre locatários gerenciados.|
|managementTemplates|[Coleção microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|A coleção de modelos de gerenciamento de linha de base entre locatários gerenciados.|
|myRoles|[Coleção microsoft.graph.managedTenants.myRole](../resources/managedtenants-myrole.md)|A coleção de atribuições de função para um usuário conectado para um locatário gerenciado.|
|tenantGroups|[Coleção microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|A coleção de um agrupamento lógico de locatários gerenciados usados pela plataforma de gerenciamento multilocatário.|
|Inquilinos|[coleção microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|A coleção de locatários associados à entidade de gerenciamento.|
|tenantsCustomizedInformation|[coleção microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|A coleção de informações personalizadas no nível do locatário entre locatários gerenciados.|
|tenantsDetailedInformation|[coleção microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|As informações detalhadas no nível do locatário da coleção entre locatários gerenciados.|
|tenantTags|[Coleção microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|A coleção de marcas de locatário entre locatários gerenciados.|
|tenantUsage|[Coleção microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md)|A coleção de uso de locatários entre locatários gerenciados.|
|windowsDeviceMalwareStates|[coleção microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md)|O estado de malware para Windows, registrado com Microsoft Endpoint Manager, entre locatários gerenciados.|
|windowsProtectionStates|[Coleção microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|O estado de proteção para Windows dispositivos, registrados com Microsoft Endpoint Manager, entre locatários gerenciados.|

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
