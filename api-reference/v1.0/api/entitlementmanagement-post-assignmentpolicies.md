---
title: Criar assignmentPolicies
description: Crie um novo objeto accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 848f259c6d40ae14fb45c9230ad4d0b524dbf17b
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608247"
---
# <a name="create-assignmentpolicies"></a>Criar assignmentPolicies
Namespace: microsoft.graph

No [gerenciamento de direitos do Azure AD](../resources/entitlementmanagement-overview.md), crie um novo [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .  A solicitação incluirá uma referência ao [accessPackage](../resources/accesspackage.md) que conterá essa política, que já deve existir.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All  |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .

Você pode especificar as seguintes propriedades ao criar **um accessPackageAssignmentPolicy**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|A descrição da política.|
|displayName|Cadeia de caracteres|O nome de exibição da política.|
|allowedTargetScope|allowedTargetScope|Who é permitido que o pacote de acesso seja atribuído por meio desta política. Os valores possíveis são `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`. Opcional.|
|expiration|[expirationPattern](../resources/expirationpattern.md)|A data de expiração das atribuições criadas nesta política.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Especifica as configurações para aprovação de solicitações para uma atribuição de pacote de acesso por meio desta política. Por exemplo, se a aprovação for necessária para novas solicitações.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Fornece configurações adicionais para selecionar quem pode criar uma solicitação para uma atribuição de pacote de acesso por meio dessa política e o que eles podem incluir em sua solicitação.|
|specificAllowedTargets|[coleção subjectSet](../resources/subjectset.md)|Os destinos para o acesso atribuído a partir de um pacote de acesso desta política.|
|accessPackage|[accessPackage](../resources/accesspackage.md)| Uma referência ao pacote de acesso que conterá a política, que já deve existir.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
Content-Type: application/json

{
  "displayName": "New Policy",
  "description": "policy for assignment",
  "allowedTargetScope": "notSpecified",
  "specificAllowedTargets": [],
  "expiration": {
      "endDateTime": null,
      "duration": null,
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": false,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": false,
      "allowCustomAssignmentSchedule": true,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": false,
      "isApprovalRequiredForUpdate": false,
      "stages": []
  },
  "accessPackage": {
      "id": "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "New policy",
  "description": "policy for assignment"
}
```


