---
title: Tipo de recurso rbacApplication
description: Propriedade de navegação de gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c3833d07e0fb9758cc8f4f5418f725889fd784dc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760922"
---
# <a name="rbacapplication-resource-type"></a>Tipo de recurso rbacApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições unificadas de função e atribuições de função para provedores RBAC do Microsoft 365. Atualmente, o "diretório" é o único aplicativo RBAC com suporte.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Crie um novo unifiedRoleAssignment postando na coleção roleAssignments. |
| [Listar roleAssignments](../api/rbacapplication-list-roleassignments.md) | [Coleção unifiedRoleAssignment](unifiedroleassignment.md) | Obter uma coleção de objetos unifiedRoleAssignment. Somente instâncias específicas podem ser consultadas, filtrando-se roleDefitionId ou principalId. |
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
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


