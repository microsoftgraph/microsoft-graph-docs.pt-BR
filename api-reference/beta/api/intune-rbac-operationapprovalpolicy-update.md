---
title: Atualizar operationApprovalPolicy
description: Atualize as propriedades de um objeto operationApprovalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d64af17564bbdb8612814576b6190ef7d741716
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630881"
---
# <a name="update-operationapprovalpolicy"></a>Atualizar operationApprovalPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/operationApprovalPolicies/{operationApprovalPolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do OperationApprovalPolicy. Essa propriedade é somente leitura.|
|displayName|String|O nome de exibição deste OperationApprovalPolicy|
|descrição|String|A descrição deste OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas deste OperationApprovalPolicy. Essa propriedade é somente leitura.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Os valores possíveis são: , , , , `deviceDelete``deviceRetireNonCompliant`, , `deviceLock`, `deviceErase`, `deviceDisableActivationLock``windowsEnrollment``compliancePolicies`, `configurationPolicies`, `appProtectionPolicies`, `policySets`, `filters`, , , `endpointSecurity`, , `apps`, , `roles``deviceResetPasscode``unknownFutureValue``scripts``deviceRetire``deviceWipe``deviceActions`|
|approverGroupIds|Conjunto de cadeias de caracteres|As IDs de grupo para os aprovadores para este OperationApprovalPolicy|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/operationApprovalPolicies/{operationApprovalPolicyId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "policyType": "deviceWipe",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "9d2caa5f-aa5f-9d2c-5faa-2c9d5faa2c9d",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "policyType": "deviceWipe",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```




