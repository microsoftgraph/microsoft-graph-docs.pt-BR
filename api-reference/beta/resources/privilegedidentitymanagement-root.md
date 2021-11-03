---
title: Privileged Identity Management
description: APIs para o Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory e as funções de recursos do Azure.
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 09d416ebe637a82f174b9668d4b9396626e0d5a3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695472"
---
# <a name="privileged-identity-management-deprecated"></a>Privileged Identity Management (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A API Privileged Identity Management (PIM) para **funções do Azure AD** foi preterida e parou de retornar dados em 31 de maio de 2021. Use a API [de gerenciamento de função](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true).
>
>A API Privileged Identity Management (PIM) para **funções de recurso do Azure** será preterida em breve. Use a nova API DE PIM REST do Azure para [funções de recurso do Azure.](/rest/api/authorization/role-eligibility-schedule-requests)

[O PIM (Privileged Identity Management) do Active Directory do Azure (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) é um serviço que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização. Isso inclui o acesso a recursos no Azure AD, recursos do Azure e outros Microsoft Online Services, como o Microsoft 365 ou o Microsoft Intune.

O Microsoft Graph fornece as seguintes APIs para gerenciar funções do Azure AD e funções de recurso do Azure:

- [APIs para funções do Azure AD](privilegedidentitymanagement-directory.md)
- [APIs para funções de recursos do Azure](privilegedidentitymanagement-resources.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
