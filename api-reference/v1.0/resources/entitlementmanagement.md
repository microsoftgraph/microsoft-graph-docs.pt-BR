---
title: Tipo de recurso entitlementManagement
description: O singleton para conter recursos de gerenciamento de direitos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db9b09efeea88ee3fc1d1dcfefab8d1ddb1c789e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242158"
---
# <a name="entitlementmanagement-resource-type"></a>Tipo de recurso entitlementManagement

O singleton de gerenciamento de direitos é o contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)e [entitlementManagementSettings](entitlementmanagementsettings.md).  Para ver uma lista completa de recursos, consulte Visão geral do gerenciamento [de direitos.](entitlementmanagement-root.md)

Herda da [entidade](entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Esse valor indica que o recurso é um singleton. Somente leitura. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackages|[Coleção accessPackage](../resources/accesspackage.md)|Pacotes de acesso.|
|assignmentRequests|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Solicitações de atribuição de pacote de acesso.|
|assignments|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Acessar atribuições de pacote.|
|catálogos|[Coleção accessPackageCatalog](../resources/accesspackagecatalog.md)|Acessar catálogos de pacotes.|
|connectedOrganizations|[Coleção connectedOrganization](../resources/connectedorganization.md)|Organizações conectadas.|
|configurações|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|Configurações de gerenciamento de direitos.|

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


