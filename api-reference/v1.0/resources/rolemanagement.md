---
title: Tipo de recurso roleManagement
description: Microsoft 365 RBAC (controle de acesso baseado em função).
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2836a8c4832d38c0e8c2e974d9eda7163c0f2313
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241650"
---
# <a name="rolemanagement-resource-type"></a>Tipo de recurso roleManagement

Namespace: microsoft.graph

Representa uma Microsoft 365 de gerenciamento de função de controle de acesso baseado em função (RBAC). Esse recurso fornece acesso a definições de função e atribuições de função que surgiram de provedores RBAC. **Os** provedores de diretório (Azure Active Directory) **e deviceManagement** (Intune) são suportados no momento.

Para saber mais, confira: 
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
|entitlementManagement|[entitlementManagement](entitlementmanagement.md)| Contêiner para todos os recursos de gerenciamento de direitos na governança de identidade do Azure AD.|

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