---
title: Criar operationApprovalPolicy
description: Crie um novo objeto operationApprovalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 921a960d4a6434a30701765a800283484a722dbb
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348056"
---
# <a name="create-operationapprovalpolicy"></a>Criar operationApprovalPolicy

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/operationApprovalPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto operationApprovalPolicy.

A tabela a seguir mostra as propriedades que são necessárias ao criar operationApprovalPolicy.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID do OperationApprovalPolicy. Essa propriedade é somente leitura.|
|displayName|String|O nome de exibição deste OperationApprovalPolicy|
|descrição|String|A descrição deste OperationApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|A última data e hora modificadas deste OperationApprovalPolicy. Essa propriedade é somente leitura.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|O tipo de política para este OperationApprovalPolicy. Os valores possíveis são: `deviceActions` , , , , , , , , `deviceWipe` , , `deviceRetire` , , , , , `deviceRetireNonCompliant` , , `deviceDelete` `deviceLock` `deviceErase` `deviceDisableActivationLock` , `windowsEnrollment` `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` , `roles` `deviceResetPasscode` `unknownFutureValue`|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|As plataformas aplicáveis para este OperationApprovalPolicy. Os valores possíveis são: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|
|approverGroupIds|Coleção String|As IDs de grupo para os aprovadores para este OperationApprovalPolicy|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/operationApprovalPolicies
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 402

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "9d2caa5f-aa5f-9d2c-5faa-2c9d5faa2c9d",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```




