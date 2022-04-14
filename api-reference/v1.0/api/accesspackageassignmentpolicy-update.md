---
title: Atualizar accessPackageAssignmentPolicy
description: Atualize as propriedades de um objeto accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bf59437cde4e33cafe7c9d6da1af24a735f17969
ms.sourcegitcommit: ca3edeed9408ee94bb12d7acf506d7317bf01d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2022
ms.locfileid: "64842339"
---
# <a name="update-accesspackageassignmentpolicy"></a>Atualizar accessPackageAssignmentPolicy

Namespace: microsoft.graph


Atualize um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.

## <a name="permissions"></a>Permissões
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
|allowedTargetScope|allowedTargetScope|Who permissão para solicitar o pacote de acesso por meio dessa política. Os valores possíveis são `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|specificAllowedTargets|[coleção subjectSet](../resources/subjectset.md)|As entidades de segurança que podem receber acesso de um pacote de acesso por meio dessa política.|
|Expiração|[expirationPattern](../resources/expirationpattern.md)|A data de validade das atribuições criadas nesta política.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Fornece configurações adicionais para selecionar quem pode criar uma solicitação para uma atribuição de pacote de acesso por meio dessa política e o que eles podem incluir em sua solicitação.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Especifica as configurações para aprovação de solicitações para uma atribuição de pacote de acesso por meio dessa política. Por exemplo, se a aprovação for necessária para novas solicitações.|
|reviewSettings|[accessPackageReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Configurações para revisões de acesso de atribuições por meio dessa política.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) atualizado no corpo da resposta.



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
  "allowedTargetScope": "allDirectoryUsers",
  "specificAllowedTargets": [],
  "expiration": {
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": true,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": true,
      "allowCustomAssignmentSchedule": false,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": true,
      "isApprovalRequiredForUpdate": false,
      "stages": [
          {
              "durationBeforeAutomaticDenial": "P2D",
              "isApproverJustificationRequired": false,
              "isEscalationEnabled": false,
              "durationBeforeEscalation": "PT0S",
              "primaryApprovers": [
                  {
                      "@odata.type": "#microsoft.graph.requestorManager",
                      "managerLevel": 1
                  }
              ],
              "fallbackPrimaryApprovers": [
                  {
                      "@odata.type": "#microsoft.graph.singleUser",
                      "userId": "e6bf4d7d-6824-4dd0-809d-5bf42d4817c2",
                      "description": "user"
                  }
              ],
              "escalationApprovers": [],
              "fallbackEscalationApprovers": []
          }
      ]
  },
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

