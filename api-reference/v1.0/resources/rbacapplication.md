---
title: Tipo de recurso rbacApplication
description: Contêiner para definições de função e atribuições de função Microsoft 365 provedores de controle de acesso baseado em função (RBAC)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eeb36364691fb31f30bde2313598b62ab06f950f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148497"
---
# <a name="rbacapplication-resource-type"></a>Tipo de recurso rbacApplication

Namespace: microsoft.graph

Contêiner de gerenciamento de função para definições unificadas de função e atribuições de função Microsoft 365 provedores de controle de acesso baseado em função (RBAC). As atribuições de função suportam apenas uma única entidade e um único escopo. Atualmente, **o diretório** é o único provedor RBAC com suporte.

## <a name="methods"></a>Métodos

Nenhum(a)

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|[Coleção unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Recurso para conceder acesso a usuários ou grupos. |
|roleDefinitions|[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Recurso que representa as funções permitidas pelos provedores RBAC e as permissões atribuídas às funções. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rbacApplication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication"
}
```
