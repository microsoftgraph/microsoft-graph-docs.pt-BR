---
title: Privileged Identity Management - recursos do Azure
description: APIs para o Privileged Identity Management do Azure AD para gerenciar recursos do Azure.
localization_priority: Priority
author: shauliu
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: b82bbd4d37b8b5d78ec85090761201ddfc13e756
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070552"
---
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management - recursos do Azure

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o [Privileged Identity Management (PIM) do Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) para recursos do Azure para configurar o fluxo de trabalho de acesso just-in-time para suas funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos e nível de recurso. Isso inclui funções internas, como Proprietário e Colaborador, além de funções RBAC personalizadas.

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>Casos de uso comuns para recursos do PIM e do Azure usando uma API REST

| Caso de uso | Recurso | Confira também |
| --- | --- | --- |
| Integrar um recurso (assinaturas, grupo de recursos, recurso, etc.) para gerenciamento de PIM, listar todos os recursos gerenciados que o solicitante tem acesso e recuperar os relacionamentos de um recurso gerenciado. | [governanceResource](governanceresource.md) | [Descoberta e gerenciamento de funções](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| Listar todas as funções de um recurso ou obter detalhes de uma função específica em um recurso especificado. | [governanceRoleDefinition](governanceroledefinition.md) |  |
| Recuperar todas as configurações de função de um recurso ou fazer uma atualização para uma configuração de função | [governanceRoleSetting](governancerolesetting.md) | [Definir configuração de função](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| Listar e exportar todas as atribuições de função de um recurso. | [governanceRoleAssignment](governanceroleassignment.md) | [Exportar atribuições de função](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| Criar ou remover uma atribuição de função elegível ou ativa, ativar/desativar uma atribuição qualificada, visualizar uma lista de solicitações pendentes, aprovar ou negar uma solicitação pendente ou cancelar sua própria solicitação pendente. | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [Atribuição de Função](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[Ativação de função](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[Aprovar solicitações](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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


