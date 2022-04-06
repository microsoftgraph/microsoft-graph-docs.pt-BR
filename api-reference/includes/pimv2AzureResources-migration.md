---
author: carolinetempleton
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: c17741c368295201dd626df91de161cf318efc1b
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477850"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-the-azure-resource-manager-arm-pim-api-for-azure-resource-roles"></a>Migrar para a API do PIM Azure Resource Manager (ARM) para funções de recurso do Azure

A API do PIM v3 para gerenciar recursos do Azure agora está disponível por meio da API REST Azure Resource Manager (ARM). Use esta orientação para migrar suas APIs existentes para as novas [APIs do Azure Resource Manager (ARM)](/rest/api/authorization/privileged-role-eligibility-rest-sample).

A tabela a seguir descreve como as novas APIs ARM são mapeadas para as APIs existentes.

| Operation | Microsoft Graph API (PIM v2) | ARM API (PIM v3) |
| --------- | ------------ | -------------- |
| Registrar um recurso | [Registrar](/graph/api/governanceresource-register) | O ARM não exige que os recursos sejam explicitamente registrados ou integrados para serem gerenciados. Você pode executar operações usando diretamente o escopo do recurso. |
| Listar definições de função | [Definições de Função de lista](/graph/api/governanceroledefinition-list) | [Definições de Função - Listar](/rest/api/authorization/role-definitions/list) |
| Criar solicitações de atribuição de função | [Criar governanceRoleAssignmentRequest](/graph/api/governanceroleassignmentrequest-post) | Usar [Solicitações de Agendamento de Qualificação de Função - Criar ](/rest/api/authorization/role-eligibility-schedule-requests/create) para criar atribuições de função qualificadas<br/><br/>Usar [Solicitações de Agendamento de Atribuição de Função - Criar](/rest/api/authorization/role-assignment-schedule-requests/create) para criar atribuições de função ativa |
| Listar atribuições de função | [Listar governanceRoleAssignments](/graph/api/governanceroleassignment-list) | Use [Instâncias de Programação de Qualificação de Função - Listar ](/rest/api/authorization/role-eligibility-schedule-instances/list-for-scope) para obter atribuições de função qualificadas<br/><br/>Usar [Instâncias de Agendamento de Atribuição de Função - Lista](/rest/api/authorization/role-assignment-schedule-instances/list-for-scope) para obter atribuições de função ativa |
| Gerenciar Configurações de Função | [Listar governanceRoleSettings](/graph/api/governancerolesetting-list)<br/>[Atualizar governanceRoleSetting](/graph/api/governancerolesetting-update) | [Gerenciar políticas por meio do ARM](/rest/api/authorization/privileged-role-policy-rest-sample)