---
title: Tipo de recurso operationApprovalPolicy
description: Política de Aprovação de Operação
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8bcee20030f654ff17f0ebba28ba199dbbe1a7c
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367899"
---
# <a name="operationapprovalpolicy-resource-type"></a>Tipo de recurso operationApprovalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Política de Aprovação de Operação

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationApprovalPolicies](../api/intune-rbac-operationapprovalpolicy-list.md)|[Coleção operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Listar propriedades e relações dos objetos [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Obter operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-get.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Leia propriedades e relações do [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Criar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-create.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Crie um novo [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[Excluir operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-delete.md)|Nenhum|Exclui uma [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).|
|[Atualizar operationApprovalPolicy](../api/intune-rbac-operationapprovalpolicy-update.md)|[operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md)|Atualize as propriedades de um [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .|
|[função getOperationsAllowedApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsallowedapproval.md)|[Coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|
|[função getOperationsRequiringApproval](../api/intune-rbac-operationapprovalpolicy-getoperationsrequiringapproval.md)|[Coleção operationApprovalPolicySet](../resources/intune-rbac-operationapprovalpolicyset.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do OperationApprovalPolicy. Essa propriedade é somente leitura.|
|displayName|String|O nome de exibição deste OperationApprovalPolicy|
|description|String|A descrição deste OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas deste OperationApprovalPolicy. Essa propriedade é somente leitura.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Os valores possíveis são: , , , , `deviceDelete``deviceRetireNonCompliant`, , `deviceLock`, `deviceErase`, `deviceDisableActivationLock``windowsEnrollment``compliancePolicies`, `configurationPolicies`, `appProtectionPolicies`, `policySets`, `filters`, , , `endpointSecurity`, , `apps`, , `roles``deviceResetPasscode``unknownFutureValue``scripts``deviceRetire``deviceWipe``deviceActions`|
|approverGroupIds|Coleção String|As IDs de grupo para os aprovadores para este OperationApprovalPolicy|

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
  "approverGroupIds": [
    "String"
  ]
}
```




