---
title: Tipo de recurso entitlementManagement
description: O contêiner para recursos de gerenciamento de direitos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c9c34a3699402f8d49fb2c0a0d9af3d5159a0eb3
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651679"
---
# <a name="entitlementmanagement-resource-type"></a>Tipo de recurso entitlementManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O singleton de gerenciamento de direitos é o contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)e [entitlementManagementSettings](entitlementmanagementsettings.md).  Para ver uma lista completa de recursos, consulte Visão geral do gerenciamento [de direitos.](entitlementmanagement-overview.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[coleção accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)| Representa a política que rege quais assuntos podem solicitar ou ser atribuídos a um pacote de acesso por meio de uma atribuição de pacote de acesso. |
|accessPackageAssignmentRequests|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Representa solicitações de atribuição de pacote de acesso criadas por ou em nome de um usuário.|
|accessPackageAssignmentResourceRoles|[Coleção accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)| Representa a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.|
|accessPackageAssignments|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Representa a concessão de um pacote de acesso a um assunto (usuário ou grupo).|
|accessPackageCatalogs|[Coleção accessPackageCatalog](../resources/accesspackagecatalog.md)|Representa um grupo de pacotes de acesso.|
|accessPackageResourceEnvironments|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)| Uma referência ao ambiente de localização geográfica no qual um recurso está localizado.|
|accessPackageResourceRequests|[Coleção accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Representa uma solicitação para adicionar ou remover um recurso para ou de um catálogo, respectivamente. |
|accessPackageResourceRoleScopes|[Coleção accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)| Uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo. |
|accessPackageResources|[Coleção accessPackageResource](../resources/accesspackageresource.md)| Uma referência a um recurso associado a um catálogo de pacotes de acesso.|
|accessPackages|[Coleção accessPackage](../resources/accesspackage.md)|Representa objetos do pacote de acesso.|
|connectedOrganizations|[Coleção connectedOrganization](../resources/connectedorganization.md)|Representa referências a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.|
|configurações|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Representa as configurações que controlam o comportamento do gerenciamento de direitos do Azure AD.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "String (identifier)"
}
```

