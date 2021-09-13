---
title: Tipo de recurso roleManagement
description: Microsoft 365 RBAC (controle de acesso baseado em função).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6f28f6e682ebba03740e5cd07d17de838d2aea18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097807"
---
# <a name="rolemanagement-resource-type"></a>Tipo de recurso roleManagement

Namespace: microsoft.graph

Representa uma Microsoft 365 de gerenciamento de função de controle de acesso baseado em função (RBAC). Esse recurso fornece acesso a definições de função e atribuições de função que surgiram de provedores RBAC. **Os** provedores de diretório (Azure Active Directory) **e deviceManagement** (Intune) são suportados no momento.

Para saber mais, consulte: 
* [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/roles/custom-overview).
* [Controle de acesso baseado em função (RBAC) com Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|directory|[rbacApplication](rbacapplication.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```