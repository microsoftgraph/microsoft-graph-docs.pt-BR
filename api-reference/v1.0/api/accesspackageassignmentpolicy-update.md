---
title: Atualizar accessPackageAssignmentPolicy
description: Atualize as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9721e20954105efde2c43be33ec47889884405e7
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608241"
---
# <a name="update-accesspackageassignmentpolicy"></a>Atualizar accessPackageAssignmentPolicy

Namespace: microsoft.graph


Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da política.|
|description|Cadeia de caracteres|A descrição da política.|
|allowedTargetScope|allowedTargetScope|Who permissão para solicitar o pacote de acesso por meio desta política. Os valores possíveis são `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|specificAllowedTargets|[coleção subjectSet](../resources/subjectset.md)|As entidades que podem ser atribuídas acesso a partir de um pacote de acesso por meio dessa política.|
|expiration|[expirationPattern](../resources/expirationpattern.md)|A data de expiração das atribuições criadas nesta política.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Fornece configurações adicionais para selecionar quem pode criar uma solicitação para uma atribuição de pacote de acesso por meio dessa política e o que eles podem incluir em sua solicitação.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Especifica as configurações para aprovação de solicitações para uma atribuição de pacote de acesso por meio desta política. Por exemplo, se a aprovação for necessária para novas solicitações.|
|reviewSettings|[accessPackageReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Configurações para ver as revisões de acesso de atribuições por meio desta política.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.



## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies/87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187
Content-Type: application/json

{
  "id":"87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "accessPackage": {
        "id": "49d2c59b-0a81-463d-a8ec-ddad3935d8a0"
  }
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory."
}
```

