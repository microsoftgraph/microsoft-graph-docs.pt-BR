---
title: Privileged Identity Management
description: APIs para o Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory e as funções de recursos do Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: acea0d13baefebe5b42833ae1bd6968705ed1c3d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136229"
---
# <a name="privileged-identity-management"></a>Privileged Identity Management

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[O PIM (Privileged Identity Management) do Active Directory do Azure (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) é um serviço que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização. Isso inclui o acesso a recursos no Azure AD, recursos do Azure e outros Microsoft Online Services, como o Microsoft 365 ou o Microsoft Intune. O Microsoft Graph fornece APIs que você pode usar para gerenciar as funções do Azure AD e as funções de recursos do Azure.

- [APIs para funções do Azure AD](privilegedidentitymanagement-directory.md)
- [APIs para funções de recursos do Azure](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> A API para gerenciar as funções do Azure Active Directory foi preterida para a maioria dos locatários, exceto para poucos que usam uma versão mais antiga da Gestão de Identidade Privilegiada (PIM). Para obter mais informações sobre as versões do PIM, confira [Determinar sua versão do PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim). Se estiver usando a nova versão e recebendo o erro **TenantEnabledInAadRoleMigration**, você pode aguardar até que uma nova API esteja disponível para a funcionalidade PIM na API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) para funções do Azure Active Directory ou você pode use a API de [Recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) para suas funções do Azure Active Directory. Para usar a API de **recurso do Azure**, substitua `azureResources` por `aadRoles` para `provider_id` e use o seu ID de locatário para `resource_id`. Recomendamos que você aguarde a nova API. Você poderá continuar usando a API de **recursos do Azure** depois que a nova API estiver disponível. Os novos recursos disponibilizados no portal do Azure também serão disponibilizados exclusivamente por meio da nova API.

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
