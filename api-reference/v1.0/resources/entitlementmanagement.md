---
title: Tipo de recurso entitlementManagement
description: O contêiner para recursos de gerenciamento de direitos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 85fb78ba5973e3493d2dd62b5e4685d0176dcbe7
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650906"
---
# <a name="entitlementmanagement-resource-type"></a>Tipo de recurso entitlementManagement

O singleton de gerenciamento de direitos é o contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)e [entitlementManagementSettings](entitlementmanagementsettings.md).  Para ver uma lista completa de recursos, consulte Visão geral do gerenciamento [de direitos.](entitlementmanagement-overview.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Esse valor indica que o recurso é um singleton. Somente leitura. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackages|[Coleção accessPackage](../resources/accesspackage.md)|Representa objetos do pacote de acesso.|
|assignmentRequests|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Representa solicitações de atribuição de pacote de acesso criadas por ou em nome de um usuário.|
|assignments|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)| Representa a concessão de um pacote de acesso a um assunto (usuário ou grupo).|
|catálogos|[Coleção accessPackageCatalog](../resources/accesspackagecatalog.md)| Representa um grupo de pacotes de acesso.|
|connectedOrganizations|[Coleção connectedOrganization](../resources/connectedorganization.md)|Representa referências a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.|
|configurações|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)| Representa as configurações que controlam o comportamento do gerenciamento de direitos do Azure AD.|

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


