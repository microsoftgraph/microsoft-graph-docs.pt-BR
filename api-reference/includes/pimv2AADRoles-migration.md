---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: ba8ba53c60d37d55cffba7b3f9626832bbf2f1cc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441697"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>Migrar para a API do PIM v3 para funções do Azure AD (APIs de gerenciamento de função)

A API do PIM para funções do Azure AD foi desativada e parou de retornar dados em 31 de maio de 2021. Use essas diretrizes para migrar suas APIs existentes para a nova [API de gerenciamento de funções para gerenciamento de identidades privilegiadas](/graph/api/resources/privilegedidentitymanagementv3-overview).

| Operation | PIM v2 API | APIs de gerenciamento de funções (PIM v3) |
| --------- | ------------ | -------------- |
| Listar definições de função | [Listar privilegedRoles](/graph/api/privilegedrole-list) | [Listar unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| Gerenciar Configurações de Função | [Get privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[Atualização de privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [Gerenciar políticas](/graph/api/policyroot-list-rolemanagementpolicies)
| Criar solicitações de atribuição de função | [Criar privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | Use [Criar unifiedRoleEligibilityScheduleRequest](/graph/api/rbacapplication-post-roleeligibilityschedulerequests) para criar atribuições de função qualificadas<br/><br/>Use [Criar unifiedRoleAssignmentScheduleRequest](/graph/api/rbacapplication-post-roleassignmentschedulerequests) para criar atribuições de função ativas |
| Listar atribuições de função | [Listar privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | Use [Listar unifiedRoleEligibilityScheduleInstances](/graph/api/rbacapplication-list-roleeligibilityscheduleinstances) para obter atribuições de função qualificadas<br/><br/>Use [Listar unifiedRoleAssignmentScheduleInstances](/graph/api/rbacapplication-list-roleassignmentscheduleinstances) para obter atribuições de função ativas |
