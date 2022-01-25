---
title: Tipo de recurso rbacApplicationMultiple
description: Propriedade de navegação de gerenciamento de função
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 963a4194b66bf901c5e724df097957272a64e2de
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201747"
---
# <a name="rbacapplicationmultiple-resource-type"></a>Tipo de recurso rbacApplicationMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para Microsoft 365 provedores RBAC que suportam várias entidades principais e vários escopos em uma única atribuição de função. Isso é diferente do tipo de recurso [rbacApplication.](rbacapplication.md)

Cloud PC e Microsoft Intune são exemplos desses provedores RBAC. Uma atribuição de função nesses provedores pode ter uma matriz de entidades e uma matriz de grupos de escopo.

Para definições de função, o provedor de computadores na nuvem atualmente dá suporte à operação [de](../api/rbacapplication-list-roledefinitions.md) lista, mas não ao [criar](../api/rbacapplication-post-roledefinitions.md).

Herda da [entidade](entity.md).

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

|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|[Coleção unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)| Recurso para conceder acesso a usuários ou grupos. |
|roleDefinitions|[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Recurso que representa as funções permitidas pelos provedores RBAC e as permissões atribuídas às funções. |

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


