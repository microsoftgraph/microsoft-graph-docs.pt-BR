---
title: Tipo de recurso rbacApplicationMultiple
description: Propriedade de navegação de gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba6c4973dd79f328c1d04ea26803a6b2aec39c7f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760915"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Tipo de recurso rbacApplicationMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores RBAC do Microsoft 365 que suportam várias entidades principais e vários escopos em uma única atribuição de função. Isso é diferente do [tipo de recurso rbacApplication.](rbacapplication.md) O Microsoft Intune é um exemplo desse provedor RBAC. Uma atribuição de função no Intune pode ter uma matriz de entidades e uma matriz de grupos de escopo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignments. |
| [Listar roleAssignmentsMultiple](../api/unifiedroleassignmentmultiple-list.md) | [Coleção unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Obter a coleção de objetos unifiedRoleAssignmentMultiple. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions. |
| [Listar roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Obter uma coleção de objetos unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Nenhum

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


