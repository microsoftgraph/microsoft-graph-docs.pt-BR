---
title: Tipo de recurso rbacApplicationMultiple
description: Propriedade de navegação de gerenciamento de função
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a989896dbf3ae71daade9e4feee07f3ea2bcd94b
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766345"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Tipo de recurso rbacApplicationMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para Microsoft 365 provedores RBAC que suportam várias entidades principais e vários escopos em uma única atribuição de função. 

Isso é diferente do [tipo de recurso rbacApplication.](rbacapplication.md) 

Cloud PC e Microsoft Intune são exemplos desses provedores RBAC. Uma atribuição de função nesses provedores pode ter uma matriz de entidades e uma matriz de grupos de escopo.

Para definições de função, o provedor de computadores na nuvem atualmente dá suporte à operação [de](../api/rbacapplication-list-roledefinitions.md) lista, mas não ao [criar](../api/rbacapplication-post-roledefinitions.md).


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions. |
| [Listar roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Obter uma coleção de objetos unifiedRoleDefinition. |
| [Criar unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignments. |
| [Listar roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md) | [Coleção unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Obter a coleção de objetos unifiedRoleAssignmentMultiple. |

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


