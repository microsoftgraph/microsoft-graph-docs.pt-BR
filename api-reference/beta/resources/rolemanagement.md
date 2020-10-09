---
title: tipo de recurso roleManagement
description: Recurso de gerenciamento de função RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 531412e826d730b634ff7506386963e0e465127b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400597"
---
# <a name="rolemanagement-resource-type"></a>tipo de recurso roleManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entidade de gerenciamento de função RBAC da Microsoft 365. Fornece acesso a definições de função e atribuições de função provenientes de provedores de RBAC. Os provedores de diretório atualmente (Azure AD) e deviceManagement (Intune) têm suporte. 

Para saber mais, confira: 
* [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* [Controle de acesso baseado em função (RBAC) com o Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Directory|[rbacApplication](rbacapplication.md)| Somente leitura. Anulável.|
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