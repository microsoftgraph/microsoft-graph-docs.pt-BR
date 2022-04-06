---
author: carolinetempleton
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: 380107ef1adb54df7452a8baa157e446cf44dd35
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "64477836"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>Migrar para a API do PIM v3 para funções do Azure AD (APIs de gerenciamento de função)

A API do PIM para funções do Azure AD foi desativada e parou de retornar dados em 31 de maio de 2021. Use esta orientação para migrar suas APIs existentes para a nova API de [gerenciamento de funções](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true).

| Operation | PIM v2 API | APIs de gerenciamento de funções (PIM v3) |
| --------- | ------------ | -------------- |
| Listar definições de função | [Listar privilegedRoles](/graph/api/privilegedrole-list) | [Listar unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| Gerenciar Configurações de Função | [Get privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[Atualização de privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [Gerenciar políticas](/graph/api/unifiedrolemanagementpolicy-list)
| Criar solicitações de atribuição de função | [Criar privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | Use [Criar unifiedRoleEligibilityScheduleRequest](/graph/api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests) para criar atribuições de função qualificadas<br/><br/>Use [Criar unifiedRoleAssignmentScheduleRequest](/graph/api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests) para criar atribuições de função ativas |
| Listar atribuições de função | [Listar privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | Use [Listar unifiedRoleEligibilityScheduleInstances](/graph/api/unifiedroleeligibilityscheduleinstance-list) para obter atribuições de função qualificadas<br/><br/>Use [Listar unifiedRoleAssignmentScheduleInstances](/graph/api/unifiedroleassignmentscheduleinstance-list) para obter atribuições de função ativas |