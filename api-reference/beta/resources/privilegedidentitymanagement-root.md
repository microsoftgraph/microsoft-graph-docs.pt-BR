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
# <a name="privileged-identity-management"></a><span data-ttu-id="d8e50-103">Privileged Identity Management</span><span class="sxs-lookup"><span data-stu-id="d8e50-103">Privileged Identity Management</span></span>

<span data-ttu-id="d8e50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8e50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8e50-105">[O PIM (Privileged Identity Management) do Active Directory do Azure (Azure AD)](/azure/active-directory/privileged-identity-management/pim-configure) é um serviço que permite gerenciar, controlar e monitorar o acesso a recursos importantes em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d8e50-105">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="d8e50-106">Isso inclui o acesso a recursos no Azure AD, recursos do Azure e outros Microsoft Online Services, como o Microsoft 365 ou o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d8e50-106">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Microsoft 365 or Microsoft Intune.</span></span> <span data-ttu-id="d8e50-107">O Microsoft Graph fornece APIs que você pode usar para gerenciar as funções do Azure AD e as funções de recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="d8e50-107">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="d8e50-108">APIs para funções do Azure AD</span><span class="sxs-lookup"><span data-stu-id="d8e50-108">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="d8e50-109">APIs para funções de recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="d8e50-109">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="d8e50-110">A API para gerenciar as funções do Azure Active Directory foi preterida para a maioria dos locatários, exceto para poucos que usam uma versão mais antiga da Gestão de Identidade Privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="d8e50-110">The API to manage Azure AD roles is deprecated for most tenants except for a few that use an older version of Privileged Identity Management (PIM).</span></span> <span data-ttu-id="d8e50-111">Para obter mais informações sobre as versões do PIM, confira [Determinar sua versão do PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span><span class="sxs-lookup"><span data-stu-id="d8e50-111">For more information about PIM versions, see [Determine your version of PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span></span> <span data-ttu-id="d8e50-112">Se estiver usando a nova versão e recebendo o erro **TenantEnabledInAadRoleMigration**, você pode aguardar até que uma nova API esteja disponível para a funcionalidade PIM na API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) para funções do Azure Active Directory ou você pode use a API de [Recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) para suas funções do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8e50-112">If you are using the new version and are recieving a **TenantEnabledInAadRoleMigration** error, you can wait until a new API is available for PIM functionality under the [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) API for Azure AD roles, or you can use the [Azure Resource](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) API for your Azure AD roles.</span></span> <span data-ttu-id="d8e50-113">Para usar a API de **recurso do Azure**, substitua `azureResources` por `aadRoles` para `provider_id` e use o seu ID de locatário para `resource_id`.</span><span class="sxs-lookup"><span data-stu-id="d8e50-113">To use the **Azure resource** API, replace `azureResources` with `aadRoles` for `provider_id` and use your tenant id for `resource_id`.</span></span> <span data-ttu-id="d8e50-114">Recomendamos que você aguarde a nova API.</span><span class="sxs-lookup"><span data-stu-id="d8e50-114">We recommend that you wait for the new API.</span></span> <span data-ttu-id="d8e50-115">Você poderá continuar usando a API de **recursos do Azure** depois que a nova API estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="d8e50-115">You will be able to continue using the **Azure resource** API after the new API is available.</span></span> <span data-ttu-id="d8e50-116">Os novos recursos disponibilizados no portal do Azure também serão disponibilizados exclusivamente por meio da nova API.</span><span class="sxs-lookup"><span data-stu-id="d8e50-116">Any new features made available in the Azure portal will also be made exclusively available through the new API.</span></span>

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
