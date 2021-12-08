---
title: Tipo de recurso operationApprovalPolicySet
description: Contém o par de OperationApprovalPolicyType e OperationApprovalPolicyPlatform determinando o conjunto de OperationApprovalPolicies aplicáveis para um usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d314a9ca5d8f842b7e898ba0ff358241bf996e2f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340169"
---
# <a name="operationapprovalpolicyset-resource-type"></a>Tipo de recurso operationApprovalPolicySet

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém o par de OperationApprovalPolicyType e OperationApprovalPolicyPlatform determinando o conjunto de OperationApprovalPolicies aplicáveis para um usuário

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Essa propriedade é somente leitura. Os valores possíveis são: `deviceActions` , , , , , , , , `deviceWipe` , , `deviceRetire` , , , , , `deviceRetireNonCompliant` , , `deviceDelete` `deviceLock` `deviceErase` `deviceDisableActivationLock` , `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` , `roles` `deviceResetPasscode` `unknownFutureValue`|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|As plataformas aplicáveis para este OperationApprovalPolicy. Essa propriedade é somente leitura. Os valores possíveis são: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalPolicySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicySet",
  "policyType": "String",
  "policyPlatform": "String"
}
```




