---
title: Privileged Identity Management
description: APIs para o Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory e as funções de recursos do Azure.
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 31f19ab4c6dbb79c5bbf60c045b3367e2d819ee9
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546074"
---
# <a name="privileged-identity-management"></a><span data-ttu-id="9b53f-103">Privileged Identity Management</span><span class="sxs-lookup"><span data-stu-id="9b53f-103">Privileged Identity Management</span></span>

<span data-ttu-id="9b53f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b53f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b53f-105">[O PIM (Privileged Identity Management) do Active Directory do Azure (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) é um serviço que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização.</span><span class="sxs-lookup"><span data-stu-id="9b53f-105">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="9b53f-106">Isso inclui o acesso a recursos no Azure AD, recursos do Azure e outros Microsoft Online Services, como o Microsoft 365 ou o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9b53f-106">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Microsoft 365 or Microsoft Intune.</span></span> <span data-ttu-id="9b53f-107">O Microsoft Graph fornece APIs que você pode usar para gerenciar as funções do Azure AD e as funções de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="9b53f-107">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="9b53f-108">APIs para funções do Azure AD</span><span class="sxs-lookup"><span data-stu-id="9b53f-108">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="9b53f-109">APIs para funções de recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="9b53f-109">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="9b53f-110">A API para gerenciar as funções do Azure Active Directory foi preterida para a maioria dos locatários, exceto para poucos que usam uma versão mais antiga da Gestão de Identidade Privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="9b53f-110">The API to manage Azure AD roles is deprecated for most tenants except for a few that use an older version of Privileged Identity Management (PIM).</span></span> <span data-ttu-id="9b53f-111">Para obter mais informações sobre as versões do PIM, confira [Determinar sua versão do PIM](/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span><span class="sxs-lookup"><span data-stu-id="9b53f-111">For more information about PIM versions, see [Determine your version of PIM](/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span></span> <span data-ttu-id="9b53f-112">Se estiver usando a nova versão e recebendo o erro **TenantEnabledInAadRoleMigration**, você pode aguardar até que uma nova API esteja disponível para a funcionalidade PIM na API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) para funções do Azure Active Directory ou você pode use a API de [Recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) para suas funções do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9b53f-112">If you are using the new version and are recieving a **TenantEnabledInAadRoleMigration** error, you can wait until a new API is available for PIM functionality under the [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) API for Azure AD roles, or you can use the [Azure Resource](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) API for your Azure AD roles.</span></span> <span data-ttu-id="9b53f-113">Para usar a API de **recurso do Azure**, substitua `azureResources` por `aadRoles` para `provider_id` e use o seu ID de locatário para `resource_id`.</span><span class="sxs-lookup"><span data-stu-id="9b53f-113">To use the **Azure resource** API, replace `azureResources` with `aadRoles` for `provider_id` and use your tenant id for `resource_id`.</span></span> <span data-ttu-id="9b53f-114">Recomendamos que você aguarde a nova API.</span><span class="sxs-lookup"><span data-stu-id="9b53f-114">We recommend that you wait for the new API.</span></span> <span data-ttu-id="9b53f-115">Você poderá continuar usando a API de **recursos do Azure** depois que a nova API estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="9b53f-115">You will be able to continue using the **Azure resource** API after the new API is available.</span></span> <span data-ttu-id="9b53f-116">Os novos recursos disponibilizados no portal do Azure também serão disponibilizados exclusivamente por meio da nova API.</span><span class="sxs-lookup"><span data-stu-id="9b53f-116">Any new features made available in the Azure portal will also be made exclusively available through the new API.</span></span>

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
