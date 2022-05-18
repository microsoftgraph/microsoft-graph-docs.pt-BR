---
title: Privileged Identity Management
description: APIs para o Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory e as funções de recursos do Azure.
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: ab02fa8a20b6f01bf0d7b71aa70882b7f0af51bb
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461280"
---
# <a name="privileged-identity-management-deprecated"></a>Privileged Identity Management (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>A API Privileged Identity Management (PIM) para **funções do Azure AD** foi preterida e parou de retornar dados em 31 de maio de 2021. Use a API de [gerenciamento de funções](/graph/api/resources/privilegedidentitymanagementv3-overview?view=graph-rest-beta&preserve-view=true) e consulte as [diretrizes de migração abaixo](#migrate-from-pim-v2-to-pim-v3-apis).
>
>A API do Privileged Identity Management (PIM) para **recursos do Azure** será preterida em breve. Use a nova [API de REST PIM do Azure para recursos do Azure](/rest/api/authorization/role-eligibility-schedule-requests). Para migrar, consulte as diretrizes de migração abaixo.

O [Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) é um serviço que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização. Esse escopo inclui acesso a recursos no Azure AD, recursos do Azure e outros serviços da Microsoft como Microsoft 365 ou Microsoft Intune.

Houve várias iterações da API do PIM nos últimos anos. Essa iteração é a segunda iteração (aqui chamada de PIM v2) e foi sucedida pelo PIM v3. Para obter mais informações sobre o histórico da API do PIM, consulte o [histórico da API PIM](/azure/active-directory/privileged-identity-management/pim-apis#pim-api-history).

O Microsoft Graph fornece as seguintes APIs do PIM v2 para gerenciar funções do Azure AD e funções de recurso do Azure. Recomendamos que você migre do PIM v2 para o PIM v3.

- [APIs para funções do Azure AD](privilegedidentitymanagement-directory.md) (preterido)
- [APIs para recursos do Azure](privilegedidentitymanagement-resources.md)

## <a name="migrate-from-pim-v2-to-pim-v3-apis"></a>Migrar de PIM v2 para APIs de PIM v3

[!INCLUDE [pimv2AADRoles-migration](../../includes/pimv2AADRoles-migration.md)]

[!INCLUDE [pimv2AzureResources-migration](../../includes/pimv2AzureResources-migration.md)]

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
