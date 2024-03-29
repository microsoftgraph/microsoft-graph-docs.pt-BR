---
title: Tipo de recurso entitlementManagement
description: O contêiner para recursos de gerenciamento de direitos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 33d5ef28494441d0bbc83d276ce74da6f9e49f8b
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608104"
---
# <a name="entitlementmanagement-resource-type"></a>Tipo de recurso entitlementManagement

O singleton de gerenciamento de direitos é o contêiner para recursos de gerenciamento de direitos, incluindo [accessPackageCatalog](accesspackagecatalog.md), [connectedOrganization](connectedorganization.md) e [entitlementManagementSettings](entitlementmanagementsettings.md).  Para ver uma lista completa de recursos, consulte [Visão geral do gerenciamento de direitos](entitlementmanagement-overview.md).

Herda de [entidade](entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Esse valor indica que o recurso é um singleton. Somente leitura. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessPackageAssignmentApprovals|[coleção approval](../resources/approval.md) | Estágios de aprovação para solicitações de atribuição.|
|accessPackages|[Coleção accessPackage](../resources/accesspackage.md)|Representa objetos do pacote de acesso.|
|assignmentPolicies|[coleção accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)|Políticas de atribuição de pacote de acesso.|
|assignmentRequests|[coleção accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)|Representa solicitações de atribuição de pacote de acesso criadas por ou em nome de um usuário.|
|assignments|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)| Representa a concessão de um pacote de acesso a um assunto (usuário ou grupo).|
|catálogos|[Coleção accessPackageCatalog](../resources/accesspackagecatalog.md)| Representa uma coleção de pacotes de acesso.|
|connectedOrganizations|[Coleção connectedOrganization](../resources/connectedorganization.md)|Representa referências a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)| Representa as configurações que controlam o comportamento do gerenciamento de direitos do Azure AD.|

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


