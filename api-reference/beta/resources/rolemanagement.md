---
title: Tipo de recurso roleManagement
description: Recurso de gerenciamento de função do RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317018"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="3b4ad-103">Tipo de recurso roleManagement</span><span class="sxs-lookup"><span data-stu-id="3b4ad-103">roleManagement resource type</span></span>

<span data-ttu-id="3b4ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b4ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b4ad-105">Representa uma Microsoft 365 de gerenciamento de função RBAC que fornece acesso a definições de função e atribuições de função que surgiram de vários provedores RBAC.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-105">Represents a Microsoft 365 RBAC role management entity that provides access to role definitions and role assignments surfaced from various RBAC providers.</span></span> 

<span data-ttu-id="3b4ad-106">A API de gerenciamento de função unificada atualmente dá suporte aos seguintes provedores RBAC em Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="3b4ad-106">The unified role management API currently supports the following RBAC providers in Microsoft 365:</span></span>
- <span data-ttu-id="3b4ad-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="3b4ad-107">cloud PC</span></span> 
- <span data-ttu-id="3b4ad-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="3b4ad-108">device management (Intune)</span></span>
- <span data-ttu-id="3b4ad-109">directory (funções de diretório do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="3b4ad-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="3b4ad-110">gerenciamento de direitos (gerenciamento de direitos do Azure AD)</span><span class="sxs-lookup"><span data-stu-id="3b4ad-110">entitlement management (Azure AD entitlement management)</span></span>
 
<span data-ttu-id="3b4ad-111">Para mais informações, confira:</span><span class="sxs-lookup"><span data-stu-id="3b4ad-111">For more information, see:</span></span> 
* [<span data-ttu-id="3b4ad-112">Funções em Microsoft 365, incluindo o Azure AD, funções específicas do serviço e entre serviços</span><span class="sxs-lookup"><span data-stu-id="3b4ad-112">Roles in Microsoft 365, including Azure AD, service-specific and cross-service roles</span></span>](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* <span data-ttu-id="3b4ad-113">[Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="3b4ad-113">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* <span data-ttu-id="3b4ad-114">Delegação e funções no gerenciamento de direitos do [Azure AD.](/azure/active-directory/governance/entitlement-management-delegate)</span><span class="sxs-lookup"><span data-stu-id="3b4ad-114">[Delegation and roles in Azure AD entitlement management](/azure/active-directory/governance/entitlement-management-delegate).</span></span>
* [<span data-ttu-id="3b4ad-115">Controle de acesso baseado em função (RBAC) com Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3b4ad-115">Role-based access control (RBAC) with Microsoft Intune</span></span>](/mem/intune/fundamentals/role-based-access-control)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="3b4ad-116">Methods</span><span class="sxs-lookup"><span data-stu-id="3b4ad-116">Methods</span></span>

<span data-ttu-id="3b4ad-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-117">None.</span></span>

## <a name="properties"></a><span data-ttu-id="3b4ad-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b4ad-118">Properties</span></span>

<span data-ttu-id="3b4ad-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="3b4ad-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3b4ad-120">Relationships</span></span>

| <span data-ttu-id="3b4ad-121">Relação</span><span class="sxs-lookup"><span data-stu-id="3b4ad-121">Relationship</span></span> | <span data-ttu-id="3b4ad-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b4ad-122">Type</span></span>        | <span data-ttu-id="3b4ad-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b4ad-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b4ad-124">cloudPC</span><span class="sxs-lookup"><span data-stu-id="3b4ad-124">cloudPC</span></span>|[<span data-ttu-id="3b4ad-125">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="3b4ad-125">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)|<span data-ttu-id="3b4ad-126">Fornece acesso a definições de função e atribuições de função de um provedor de RBAC de computador na nuvem.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-126">Provides access to role definitions and role assignments of a cloud PC RBAC provider.</span></span> <span data-ttu-id="3b4ad-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-127">Read-only.</span></span> <span data-ttu-id="3b4ad-128">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-128">Nullable.</span></span>|
|<span data-ttu-id="3b4ad-129">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3b4ad-129">deviceManagement</span></span>|[<span data-ttu-id="3b4ad-130">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="3b4ad-130">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="3b4ad-131">Fornece acesso a definições de função e atribuições de função de um provedor do Intune RBAC.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-131">Provides access to role definitions and role assignments of an Intune RBAC provider.</span></span> <span data-ttu-id="3b4ad-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-132">Read-only.</span></span> <span data-ttu-id="3b4ad-133">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-133">Nullable.</span></span>|
|<span data-ttu-id="3b4ad-134">directory</span><span class="sxs-lookup"><span data-stu-id="3b4ad-134">directory</span></span>|[<span data-ttu-id="3b4ad-135">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="3b4ad-135">rbacApplication</span></span>](rbacapplication.md)|<span data-ttu-id="3b4ad-136">Fornece acesso a definições de função e atribuições de função de um provedor do Azure AD RBAC.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-136">Provides access to role definitions and role assignments of an Azure AD RBAC provider.</span></span> <span data-ttu-id="3b4ad-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-137">Read-only.</span></span> <span data-ttu-id="3b4ad-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-138">Nullable.</span></span>|
|<span data-ttu-id="3b4ad-139">entitlementManagement</span><span class="sxs-lookup"><span data-stu-id="3b4ad-139">entitlementManagement</span></span>|[<span data-ttu-id="3b4ad-140">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="3b4ad-140">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="3b4ad-141">Fornece acesso a definições de função e atribuições de função do gerenciamento de direitos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-141">Provides access to role definitions and role assignments of Azure AD entitlement management.</span></span> <span data-ttu-id="3b4ad-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-142">Read-only.</span></span> <span data-ttu-id="3b4ad-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3b4ad-143">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b4ad-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b4ad-144">JSON representation</span></span>

<span data-ttu-id="3b4ad-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b4ad-145">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
