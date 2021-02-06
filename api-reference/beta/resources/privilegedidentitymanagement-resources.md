---
title: Privileged Identity Management - recursos do Azure
description: APIs para o Privileged Identity Management do Azure AD para gerenciar recursos do Azure.
localization_priority: Priority
author: shauliu
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: a64a60258369226ca58c4be070494e20f0d1403a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136544"
---
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="219d3-103">Privileged Identity Management - recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="219d3-103">Privileged Identity Management - Azure resources</span></span>

<span data-ttu-id="219d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="219d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="219d3-105">Você pode usar o [Privileged Identity Management (PIM) do Azure Active Directory (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) para recursos do Azure para configurar o fluxo de trabalho de acesso just-in-time para suas funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos e nível de recurso.</span><span class="sxs-lookup"><span data-stu-id="219d3-105">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="219d3-106">Isso inclui funções internas, como Proprietário e Colaborador, além de funções RBAC personalizadas.</span><span class="sxs-lookup"><span data-stu-id="219d3-106">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="219d3-107">Casos de uso comuns para recursos do PIM e do Azure usando uma API REST</span><span class="sxs-lookup"><span data-stu-id="219d3-107">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="219d3-108">Caso de uso</span><span class="sxs-lookup"><span data-stu-id="219d3-108">Use case</span></span> | <span data-ttu-id="219d3-109">Recurso</span><span class="sxs-lookup"><span data-stu-id="219d3-109">Resource</span></span> | <span data-ttu-id="219d3-110">Confira também</span><span class="sxs-lookup"><span data-stu-id="219d3-110">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="219d3-111">Integrar um recurso (assinaturas, grupo de recursos, recurso, etc.) para gerenciamento de PIM, listar todos os recursos gerenciados que o solicitante tem acesso e recuperar os relacionamentos de um recurso gerenciado.</span><span class="sxs-lookup"><span data-stu-id="219d3-111">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="219d3-112">governanceResource</span><span class="sxs-lookup"><span data-stu-id="219d3-112">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="219d3-113">Descoberta e gerenciamento de funções</span><span class="sxs-lookup"><span data-stu-id="219d3-113">Role discovery and management</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="219d3-114">Listar todas as funções de um recurso ou obter detalhes de uma função específica em um recurso especificado.</span><span class="sxs-lookup"><span data-stu-id="219d3-114">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="219d3-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="219d3-115">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="219d3-116">Recuperar todas as configurações de função de um recurso ou fazer uma atualização para uma configuração de função</span><span class="sxs-lookup"><span data-stu-id="219d3-116">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="219d3-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="219d3-117">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="219d3-118">Definir configuração de função</span><span class="sxs-lookup"><span data-stu-id="219d3-118">Configure role setting</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="219d3-119">Listar e exportar todas as atribuições de função de um recurso.</span><span class="sxs-lookup"><span data-stu-id="219d3-119">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="219d3-120">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="219d3-120">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="219d3-121">Exportar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="219d3-121">Export role assignments</span></span>](/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="219d3-122">Criar ou remover uma atribuição de função elegível ou ativa, ativar/desativar uma atribuição qualificada, visualizar uma lista de solicitações pendentes, aprovar ou negar uma solicitação pendente ou cancelar sua própria solicitação pendente.</span><span class="sxs-lookup"><span data-stu-id="219d3-122">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="219d3-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="219d3-123">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="219d3-124">Atribuição de Função</span><span class="sxs-lookup"><span data-stu-id="219d3-124">Role Assignment</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="219d3-125">Ativação de função</span><span class="sxs-lookup"><span data-stu-id="219d3-125">Role activation</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="219d3-126">Aprovar solicitações</span><span class="sxs-lookup"><span data-stu-id="219d3-126">Approve requests</span></span>](/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
