---
title: 'cloudPcProvisioningPolicy: assign'
description: Atribua a política de provisionamento do computador de nuvem ao grupo.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 3e83fa363eeec142c194865da0bb0bef191aae50
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378212"
---
# <a name="cloudpcprovisioningpolicy-assign"></a>cloudPcProvisioningPolicy: assign

Namespace: microsoft.graph

Atribuir [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) a grupos de usuários.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da atribuição de política de provisionamento. Se target for um grupo de usuários, a ID será mostrada como {PolicyId} _ {GroupId}. |
|destino|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|O destino da atribuição para a política de provisionamento. Atualmente, o único destino suportado é um grupo de usuários.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "assign_cloudpcprovisioningpolicy",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
