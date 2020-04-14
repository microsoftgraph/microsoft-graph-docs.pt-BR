---
title: tipo de recurso rbacApplicationMultiple
description: Propriedade de navegação gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6450852f63b08b6413681579e77850488106e3c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462224"
---
# <a name="rbacapplicationmultiple-resource-type"></a>tipo de recurso rbacApplicationMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores Microsoft 365 RBAC que oferecem suporte a várias entidades e vários escopos em uma única atribuição de função. Isso é diferente do tipo de recurso [rbacApplication](rbacapplication.md) . O Microsoft Intune é um exemplo de um provedor RBAC. Uma atribuição de função no Intune pode ter uma matriz de entidades e uma matriz de grupos de escopo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignments. |
| [Listar roleAssignmentsMultiple](../api/unifiedroleassignmentmultiple-list.md) | coleção [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | Obtém a coleção de objetos unifiedRoleAssignmentMultiple. Somente instâncias específicas podem ser consultadas, por meio da filtragem em unifiedRoleDefitionId ou entidade de segurança. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions. |
| [Listar roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | coleção [unifiedRoleDefinition](unifiedroledefinition.md) | Obtenha uma coleção de objetos unifiedRoleDefinition. |

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

None

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->