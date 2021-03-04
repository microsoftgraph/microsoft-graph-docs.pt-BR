---
title: Tipo de recurso roleManagement
description: Recurso de gerenciamento de função do RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440120"
---
# <a name="rolemanagement-resource-type"></a>Tipo de recurso roleManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entidade de gerenciamento de função do Microsoft 365 RBAC. Fornece acesso a definições de função e atribuições de função que surgiram de provedores RBAC. Atualmente, há suporte para provedores de diretório (Azure AD) e deviceManagement (Intune). 

Para saber mais, confira: 
* [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Controle de acesso baseado em função (RBAC) com o Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|directory|[rbacApplication](rbacapplication.md)| Somente leitura. Anulável.|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Nenhum

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
