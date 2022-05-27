---
title: tipo de recurso entitlementManagement
description: O contêiner para recursos de gerenciamento de direitos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2768db11986466e864884d611877cf93dab6ef1a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694894"
---
# <a name="entitlementmanagement-resource-type"></a>tipo de recurso entitlementManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O singleton de gerenciamento de direitos é o contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog](accesspackagecatalog.md), [connectedOrganization](connectedorganization.md) e [entitlementManagementSettings](entitlementmanagementsettings.md).  Para obter uma lista completa de recursos, consulte a [visão geral do gerenciamento de direitos](entitlementmanagement-overview.md).

Herda de [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[coleção accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)| Representa a política que rege quais assuntos podem solicitar ou receber um pacote de acesso por meio de uma atribuição de pacote de acesso. |
|accessPackageAssignmentRequests|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Representa solicitações de atribuição de pacote de acesso criadas por ou em nome de um usuário.|
|accessPackageAssignmentResourceRoles|[coleção accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)| Representa a função específica do recurso à qual uma entidade foi atribuída por meio de uma atribuição de pacote de acesso.|
|accessPackageAssignments|[coleção accessPackageAssignment](../resources/accesspackageassignment.md)|A atribuição de um pacote de acesso a um assunto por um período de tempo.|
|accessPackageCatalogs|[coleção accessPackageCatalog](../resources/accesspackagecatalog.md)|Um contêiner de pacotes de acesso.|
|accessPackageResourceEnvironments|[coleção accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)| Uma referência ao ambiente de geolocalização no qual um recurso está localizado.|
|accessPackageResourceRequests|[coleção accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Representa uma solicitação para adicionar ou remover um recurso de ou para um catálogo, respectivamente. |
|accessPackageResourceRoleScopes|[coleção accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)| Uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo. |
|accessPackageResources|[Coleção accessPackageResource](../resources/accesspackageresource.md)| Uma referência a um recurso associado a um catálogo de pacotes de acesso.|
|accessPackages|[Coleção accessPackage](../resources/accesspackage.md)|Representa objetos do pacote de acesso.|
|connectedOrganizations|[coleção connectedOrganization](../resources/connectedorganization.md)|Representa referências a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Representa as configurações que controlam o comportamento do Azure AD gerenciamento de direitos.|

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

