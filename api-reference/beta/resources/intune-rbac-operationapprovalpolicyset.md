---
title: Tipo de recurso operationApprovalPolicySet
description: Contém o par de OperationApprovalPolicyType e OperationApprovalPolicyPlatform determinando o conjunto de OperationApprovalPolicies aplicáveis para um usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54ba00c62c6618d10dbc81cfc9587a4204f0f368
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493786"
---
# <a name="operationapprovalpolicyset-resource-type"></a>Tipo de recurso operationApprovalPolicySet

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém o par de OperationApprovalPolicyType e OperationApprovalPolicyPlatform determinando o conjunto de OperationApprovalPolicies aplicáveis para um usuário

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Essa propriedade é somente leitura. Os valores possíveis são: `deviceActions` , , , , , , , , , `deviceWipe` , , , , `deviceRetire` , , , `deviceRetireNonCompliant` , `deviceDelete` `deviceLock` , `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` . `roles` `unknownFutureValue`|
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



