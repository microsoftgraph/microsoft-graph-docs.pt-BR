---
title: 'accessPackage: getApplicablePolicyRequirements'
description: Permitir que os chamadores encontrem requisitos para solicitar uma atribuição para um accessPackage específico.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2572239463e9ab1142c2b5e475f25e7ce1914b39
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259202"
---
# <a name="accesspackage-getapplicablepolicyrequirements"></a>accessPackage: getApplicablePolicyRequirements
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)essa ação recupera uma lista de objetos [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) que o usuário atualmente está assinado pode usar para criar um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).  Cada objeto de requisito corresponde a uma política de atribuição de pacote de acesso para a que o usuário atualmente está autorizado a solicitar uma atribuição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/getApplicablePolicyRequirements
```

## <a name="function-parameters"></a>Parâmetros de função

Nenhum.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md) no corpo da resposta, um objeto para cada política para a qual o usuário é **um allowedRequestor**. Se houver uma política sem requisitos, **o accessPackageAssignmentRequestRequirements** terá `false` e `null` valores. Se não houver políticas em que o usuário seja **um allowedRequestor**, uma coleção vazia será retornada.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "accesspackage_getapplicablepolicyrequirements"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/fb449cf8-3a59-4d86-bdfd-a1b7299681de/getApplicablePolicyRequirements
```

### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequestRequirements)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "policyId": "449feb20-7040-499a-ba91-bdfb93ede34b", 
            "policyDisplayName": "Initial Policy", 
            "policyDescription": "Initial Policy", 
            "isApprovalRequired": false, 
            "isApprovalRequiredForExtension": false, 
            "isRequestorJustificationRequired": false, 
            "questions": [], 
            "existingAnswers": [],
            "schedule": []
        }
    ]
}
``` 
