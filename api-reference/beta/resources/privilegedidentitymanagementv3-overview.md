---
title: Visão geral do gerenciamento de funções por meio da API pim (privileged identity management)
description: Privileged Identity Management (PIM) é um recurso do Azure AD Identity Governance que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f254a6ced18f29496ba297c3fe481d75121f9ad7
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461665"
---
# <a name="overview-of-role-management-through-the-privileged-identity-management-pim-api"></a>Visão geral do gerenciamento de funções por meio da API pim (privileged identity management)

Privileged Identity Management (PIM) é um recurso do [Azure AD Identity Governance](/azure/active-directory/governance/identity-governance-overview) que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização. Esse acesso é habilitado por meio de funções privilegiadas e RBAC (controle de acesso baseado em função) e pode ser concedido a usuários, grupos ou entidades de serviço. Os recursos podem estar em Azure AD, no Azure e em outros serviços de nuvem da Microsoft, como Microsoft 365 ou Microsoft Intune.

A API Graph PIM da Microsoft para gerenciamento de funções permite que você controle o acesso privilegiado e limite o acesso excessivo. Este artigo apresenta os recursos de governança das APIs do PIM no Microsoft Graph.

> [!NOTE]
> Para gerenciar funções de recurso do Azure, use as [APIs do ARM (Azure Resource Manager) para PIM](/rest/api/authorization/privileged-role-eligibility-rest-sample).

## <a name="pim-api-for-managing-role-assignments"></a>API do PIM para gerenciar atribuições de função

O PIM permite que você gerencie atribuições de função ativas criando atribuições permanentes ou temporárias. Use o [tipo de recurso unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) e seus métodos relacionados para gerenciar atribuições de função.

A tabela a seguir lista cenários para usar o PIM para gerenciar atribuições de função e as APIs a serem chamadas.

|Cenários  |API  |
|---------|---------|
|Um administrador cria e atribui a uma entidade de segurança uma atribuição de função permanente  <br/> Um administrador atribui a uma entidade de segurança uma função temporária   |   [Criar roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Um administrador renova, atualiza, estende ou remove atribuições de função     |   [Criar roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Um administrador consulta todas as atribuições de função e seus detalhes     |   [Listar roleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)      |
|Um administrador consulta uma atribuição de função e seus detalhes     |   [Obter unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)      |
|Uma entidade de segurança consulta suas atribuições de função e os detalhes     |  [unifiedRoleAssignmentScheduleRequest: filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)       |
|Uma entidade de segurança executa a ativação just-in-time e com limite de tempo de sua *atribuição de função qualificada*     |   [Criar roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Uma entidade de segurança cancela uma solicitação de atribuição de função que criou     |   [unifiedRoleAssignmentScheduleRequest: cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)      |
|Uma entidade de segurança que ativou sua atribuição de função qualificada a desativa quando não precisa mais de acesso     |   [Criar roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|Uma entidade de segurança desativa, estende ou renova sua própria atribuição de função.     |   [Criar roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |

## <a name="pim-api-for-managing-role-eligibilities"></a>API do PIM para gerenciar eligibilidades de função

Suas entidades de segurança podem não exigir atribuições de função permanentes porque podem não exigir os privilégios concedidos por meio da função com privilégios o tempo todo. Nesse caso, o PIM também permite criar eligibilidades de função e atribuí-las às entidades de segurança. Com as eligibilidades de função, a entidade de segurança ativa a função quando precisa executar tarefas privilegiadas. A ativação sempre tem limite de tempo por um máximo de 8 horas. A elegibilidade de função também pode ser uma qualificação permanente ou uma qualificação temporária.

Use o [tipo de recurso unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) e seus métodos relacionados para gerenciar as eligibilidades de função.

A tabela a seguir lista cenários para usar o PIM para gerenciar as eligibilidades de função e as APIs a serem chamadas.

|Cenários  |API  |
|---------|---------|
|Um administrador cria e atribui a uma entidade de segurança uma função qualificada  <br/> Um administrador atribui uma qualificação de função temporária a uma entidade de segurança   |   [Criar roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|Um administrador renova, atualiza, estende ou remove as eligibilidades de função     |   [Criar roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|Um administrador consulta todas as eligibilidades de função e seus detalhes     |   [Listar roleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)      |
|Um administrador consulta uma qualificação de função e seus detalhes     |   [Obter unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)      |
|Um administrador cancela uma solicitação de qualificação de função que ele criou     |   [unifiedRoleEligibilityScheduleRequest: cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)      |
|Uma entidade de segurança consulta suas eligibilidades de função e os detalhes     |  [unifiedRoleEligibilityScheduleRequest: filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)       |
|Uma entidade de segurança desativa, estende ou renova sua própria qualificação de função.     |   [Criar roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |


## <a name="role-settings-and-pim"></a>Configurações de função e PIM

Cada Azure AD função define configurações ou regras. Essas configurações incluem se a autenticação multifator (MFA), a justificativa ou a aprovação são necessárias para ativar uma função qualificada ou se você pode criar atribuições permanentes ou eligibilidades para entidades de segurança para a função. Essas configurações específicas de função determinarão as configurações que você pode aplicar ao criar ou gerenciar atribuições de função e eligibilidades por meio do PIM. No Microsoft Graph, essas configurações de função são gerenciadas por meio dos tipos de recursos [unifiedRoleManagementPolicyAssignment e unifiedRoleManagementPolicyAssignment](unifiedrolemanagementpolicyassignment.md) e seus métodos relacionados.[](unifiedrolemanagementpolicy.md)

Por exemplo, suponha que, por padrão, uma função não permita atribuições ativas permanentes e defina um máximo de 15 dias para atribuições ativas. A tentativa de criar um objeto [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) `400 Bad Request` sem data de expiração retornará um código de resposta para violação da regra de expiração.

A tabela a seguir lista cenários para usar o PIM para gerenciar Azure AD configurações de função ou regras e as APIs a serem chamadas.

|Cenários  |API  |
|---------|---------|
|Recuperar políticas de gerenciamento de função e regras ou configurações associadas   |   [Listar unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)      |
|Recuperar uma política de gerenciamento de função e suas regras ou configurações associadas |   [Obter unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)      |
|Recuperar as regras ou configurações definidas para a política de gerenciamento de função | [Listar regras](../api/unifiedrolemanagementpolicy-list-rules.md)       |
|Recuperar uma regra ou configurações definidas para uma política de gerenciamento de função |  [Obter unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)      |
|Atualizar uma regra ou configuração definida para uma política de gerenciamento de função|[Atualizar unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|
|Obtenha os detalhes de todas as atribuições de política de gerenciamento de função, incluindo as políticas e regras ou configurações associadas às Azure AD funções |  [Listar unifiedRoleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)      |
|Obter os detalhes de uma atribuição de política de gerenciamento de função, incluindo a política e as regras ou as configurações associadas à Azure AD função |   [Obter unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)     |

Para obter mais informações sobre configurações de função, [consulte Definir Azure AD configurações de função no Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-how-to-change-default-settings).

## <a name="pim-and-identity-security-with-zero-trust"></a>PIM e segurança de identidade com Confiança Zero

As APIs do PIM dão suporte às organizações para adotar uma Confiança Zero para proteger as identidades em sua organização. Para obter mais informações sobre Confiança Zero, consulte [Protegendo a identidade com Confiança Zero](/security/zero-trust/deploy/identity).

## <a name="permissions-and-privileges"></a>Permissões e privilégios

Para chamar as APIs [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) e [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) com ações de administrador, o usuário chamador deve:
+ Ter uma função *de Administrador Global ou* *Administrador de Função Com* Privilégios
+ Receber uma das seguintes permissões:
  + RoleAssignmentSchedule.ReadWrite.Directory
  + RoleEligibilitySchedule.ReadWrite.Directory
  + RoleManagement.ReadWrite.Directory

A entidade de segurança também deve receber as permissões apropriadas para recuperar suas atribuições de função e eligibilidades ou chamar as APIs [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) e [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) com ações do usuário.

Para obter mais informações sobre permissões para chamar APIs do PIM, consulte a referência de permissões do [Microsoft Graph: permissões de gerenciamento de função](/graph/permissions-reference#role-management-permissions).

## <a name="licensing"></a>Licenciamento

A API do PIM requer Azure AD Premium P2 licença. Para obter mais informações, consulte [Requisitos de licença para usar Privileged Identity Management](/azure/active-directory/privileged-identity-management/subscription-requirements).

## <a name="see-also"></a>Confira também

+ [O que é o Azure AD Privileged Identity Management?](/azure/active-directory/privileged-identity-management/pim-configure)
+ [Tutorial: Usar a API Privileged Identity Management (PIM) para atribuir Azure AD funções](/graph/tutorial-assign-azureadroles)
+ Você também pode configurar revisões de acesso de atribuições de função e eligibilidades gerenciadas por meio do PIM. Para obter mais informações, consulte [Tutorial: Usar a API Privileged Identity Management (PIM) para atribuir Azure AD funções](/graph/tutorial-assign-azureadroles).