---
title: Tipo de recurso accessPackageAssignmentPolicy
description: Uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ser atribuídos um pacote de acesso por meio de uma atribuição de pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 90f2b6024e63325a1e0c7e6d8156fa40189736b9
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608266"
---
# <a name="accesspackageassignmentpolicy-resource-type"></a>Tipo de recurso accessPackageAssignmentPolicy

Namespace: microsoft.graph

No [gerenciamento de direitos do Azure AD](entitlementmanagement-overview.md), uma política de atribuição de pacote de acesso especifica a política pela qual os titulares podem solicitar ou ter um pacote de acesso atribuído por meio de uma atribuição de pacote de acesso. Um pacote de acesso pode ter zero ou mais políticas. Quando uma solicitação de um assunto é recebida, o assunto é corresponder a cada política para encontrar a política (se alguma) com **requestorSettings** que incluem esse assunto. Em seguida, a política determina se a solicitação requer aprovação, a duração da atribuição do pacote de acesso e se a atribuição precisa de revisões regulares.

Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackageAssignmentPolicies](../api/entitlementmanagement-list-assignmentpolicies.md)|[coleção accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Obter uma lista dos [objetos accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) e suas propriedades.|
|[Criar accessPackageAssignmentPolicy](../api/entitlementmanagement-post-assignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Crie um novo [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Obter accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Leia as propriedades e as relações de um [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Atualizar accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Atualize as propriedades de [um objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|
|[Excluir accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md)|Nenhum|Exclui um [objeto accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowedTargetScope|allowedTargetScope|Entidades que podem ser atribuídas ao pacote de acesso por meio desta política. Os valores possíveis são `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|description|Cadeia de caracteres|A descrição da política.|
|displayName|Cadeia de caracteres|O nome de exibição da política.|
|expiration|[expirationPattern](../resources/expirationpattern.md)|A data de expiração das atribuições criadas nesta política.|
|id|Cadeia de caracteres|Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Especifica as configurações para aprovação de solicitações para uma atribuição de pacote de acesso por meio desta política. Por exemplo, se a aprovação for necessária para novas solicitações.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Fornece configurações adicionais para selecionar quem pode criar uma solicitação para uma atribuição de pacote de acesso por meio dessa política e o que eles podem incluir em sua solicitação.|
|reviewSettings|[accessPackageAssignmentReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Configurações para ver as revisões de acesso de atribuições por meio desta política.|
|specificAllowedTargets|[coleção subjectSet](../resources/subjectset.md)|As entidades que podem ser atribuídas acesso a partir de um pacote de acesso por meio dessa política.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|Pacote de acesso que contém essa política. Somente leitura. |
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Catálogo do pacote de acesso que contém essa política. Somente leitura.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "allowedTargetScope": "String",
  "specificAllowedTargets": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "requestorSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentRequestorSettings"
  },
  "requestApprovalSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentApprovalSettings"
  },
  "reviewSettings": {
    "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
  },
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


