---
title: Tipo de recurso roleManagement
description: Recurso de gerenciamento de função do RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317018"
---
# <a name="rolemanagement-resource-type"></a>Tipo de recurso roleManagement

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma Microsoft 365 de gerenciamento de função RBAC que fornece acesso a definições de função e atribuições de função que surgiram de vários provedores RBAC. 

A API de gerenciamento de função unificada atualmente dá suporte aos seguintes provedores RBAC em Microsoft 365:
- cloud PC 
- gerenciamento de dispositivos (Intune)
- directory (funções de diretório do Azure AD)
- gerenciamento de direitos (gerenciamento de direitos do Azure AD)
 
Para mais informações, confira: 
* [Funções em Microsoft 365, incluindo o Azure AD, funções específicas do serviço e entre serviços](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).
* Delegação e funções no gerenciamento de direitos do [Azure AD.](/azure/active-directory/governance/entitlement-management-delegate)
* [Controle de acesso baseado em função (RBAC) com Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|Fornece acesso a definições de função e atribuições de função de um provedor de RBAC de computador na nuvem. Somente leitura. Anulável.|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| Fornece acesso a definições de função e atribuições de função de um provedor do Intune RBAC. Somente leitura. Anulável.|
|directory|[rbacApplication](rbacapplication.md)|Fornece acesso a definições de função e atribuições de função de um provedor do Azure AD RBAC. Somente leitura. Anulável.|
|entitlementManagement|[rbacApplication](rbacapplication.md)| Fornece acesso a definições de função e atribuições de função do gerenciamento de direitos do Azure AD. Somente leitura. Anulável.|

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
