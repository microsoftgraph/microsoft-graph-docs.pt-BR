---
title: Tipo de recurso operationApprovalPolicy
description: Política de Aprovação de Operação
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45076a2f7b7e4354a7df06182904887c1147ecaa
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211302"
---
# <a name="operationapprovalpolicy-resource-type"></a>Tipo de recurso operationApprovalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de Aprovação de Operação

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[coleção operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Listar propriedades e relações dos [objetos operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Obter operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Ler propriedades e relações do objeto [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Criar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Crie um novo [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Excluir operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|Nenhuma|Exclui uma [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).|
|[Atualizar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Atualize as propriedades de [um objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Função getApprovableOperations](../api/intune-rbac-operationapprovalpolicy-getapprovableoperations.md)|[coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|
|[Função getOperationsRequiringApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da OperationApprovalPolicy. Essa propriedade é somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição desta OperationApprovalPolicy|
|descrição|Cadeia de caracteres|A descrição deste OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|A data e a hora da última modificação desta OperationApprovalPolicy. Essa propriedade é somente leitura.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Os valores possíveis são: , , , , , , `deviceLock`, , `deviceErase`, `windowsEnrollment``deviceDisableActivationLock`, `compliancePolicies`, `configurationPolicies`, , `policySets``appProtectionPolicies`, `filters`, , , `endpointSecurity`, , `apps`, , , . `unknownFutureValue``deviceResetPasscode``roles``scripts``deviceDelete``deviceRetireNonCompliant``deviceRetire``deviceWipe``deviceActions`|
|approverGroupIds|Coleção de cadeias de caracteres|As IDs de grupo para os aprovadores desta OperationApprovalPolicy|

## <a name="relationships"></a>Relações
Nenhuma

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
  "approverGroupIds": [
    "String"
  ]
}
```




