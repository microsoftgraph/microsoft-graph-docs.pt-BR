---
title: Tipo de recurso operationApprovalPolicy
description: Política de Aprovação de Operação
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d2da950900e621d4f0a50b03c86c144d36dea412
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487361"
---
# <a name="operationapprovalpolicy-resource-type"></a>Tipo de recurso operationApprovalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de Aprovação de Operação

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[Coleção operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Listar propriedades e relações dos objetos [operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Obter operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Leia propriedades e relações do [objeto operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Criar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Crie um novo [objeto operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[Excluir operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|Nenhum|Exclui uma [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).|
|[Atualizar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Atualize as propriedades de um [objeto operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)|
|[função getOperationsAllowedApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsallowedapproval.md)|[Coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|
|[função getOperationsRequiringApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[Coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do OperationApprovalPolicy. Essa propriedade é somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição deste OperationApprovalPolicy|
|description|Cadeia de caracteres|A descrição deste OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas deste OperationApprovalPolicy. Essa propriedade é somente leitura.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Os valores possíveis são: `deviceActions` , , , , , , , , , `deviceWipe` , , , , `deviceRetire` , , , `deviceRetireNonCompliant` , `deviceDelete` `deviceLock` , `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` . `roles` `unknownFutureValue`|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|As plataformas aplicáveis para este OperationApprovalPolicy. Os valores possíveis são: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|
|approverGroupIds|Coleção de cadeias de caracteres|As IDs de grupo para os aprovadores para este OperationApprovalPolicy|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyType": "String",
  "policyPlatform": "String",
  "approverGroupIds": [
    "String"
  ]
}
```



