---
title: Tipo de recurso roleManagement
description: Microsoft 365 RBAC (controle de acesso baseado em função).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 055e90c1fe006cf7babfdea4f7c585d66ff295d0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394506"
---
# <a name="rolemanagement-resource-type"></a>Tipo de recurso roleManagement

Namespace: microsoft.graph

Representa uma Microsoft 365 de gerenciamento de função de controle de acesso baseado em função (RBAC). Esse recurso fornece acesso a definições de função e atribuições de função que surgiram de provedores RBAC. **Os** provedores de diretório (Azure Active Directory), **direitoManagement** e **deviceManagement** (Intune) são suportados no momento.

Para mais informações, confira: 
* [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/roles/custom-overview).
* [Delegação e funções no gerenciamento de direitos do Azure AD](/azure/active-directory/governance/entitlement-management-delegate).
* [Controle de acesso baseado em função (RBAC) com Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|directory|[rbacApplication](rbacapplication.md)| Somente leitura. Anulável.|
|entitlementManagement|[rbacApplication](rbacapplication.md)| Contêiner para funções e atribuições para [recursos de gerenciamento de direitos](entitlementmanagement.md) .|

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