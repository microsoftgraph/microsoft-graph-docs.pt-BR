---
title: Tipo de recurso rbacApplication
description: Contêiner para definições de função e atribuições de função para Microsoft 365 RBAC (controle de acesso baseado em função)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 294bf357465002a180549e5654fbfd7f2baabac6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393470"
---
# <a name="rbacapplication-resource-type"></a>Tipo de recurso rbacApplication

Namespace: microsoft.graph

Contêiner de gerenciamento de função para definições unificadas de função e atribuições de função Microsoft 365 provedores de controle de acesso baseado em função (RBAC). As atribuições de função suportam apenas uma única entidade e um único escopo. Atualmente, **o diretório** **e o direitoManagement** são os dois provedores RBAC suportados.

## <a name="methods"></a>Methods

Nenhum

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
