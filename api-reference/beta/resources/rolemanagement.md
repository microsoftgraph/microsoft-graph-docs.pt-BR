---
title: Tipo de recurso roleManagement
description: Recurso de gerenciamento de função do RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440120"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="e47b3-103">Tipo de recurso roleManagement</span><span class="sxs-lookup"><span data-stu-id="e47b3-103">roleManagement resource type</span></span>

<span data-ttu-id="e47b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e47b3-105">Representa uma entidade de gerenciamento de função do Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="e47b3-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="e47b3-106">Fornece acesso a definições de função e atribuições de função que surgiram de provedores RBAC.</span><span class="sxs-lookup"><span data-stu-id="e47b3-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="e47b3-107">Atualmente, há suporte para provedores de diretório (Azure AD) e deviceManagement (Intune).</span><span class="sxs-lookup"><span data-stu-id="e47b3-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="e47b3-108">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="e47b3-108">For more information, see:</span></span> 
* <span data-ttu-id="e47b3-109">[Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="e47b3-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="e47b3-110">Controle de acesso baseado em função (RBAC) com o Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e47b3-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="e47b3-111">Methods</span><span class="sxs-lookup"><span data-stu-id="e47b3-111">Methods</span></span>

<span data-ttu-id="e47b3-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e47b3-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="e47b3-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e47b3-113">Properties</span></span>

<span data-ttu-id="e47b3-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e47b3-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e47b3-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e47b3-115">Relationships</span></span>

| <span data-ttu-id="e47b3-116">Relação</span><span class="sxs-lookup"><span data-stu-id="e47b3-116">Relationship</span></span> | <span data-ttu-id="e47b3-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="e47b3-117">Type</span></span>        | <span data-ttu-id="e47b3-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="e47b3-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e47b3-119">directory</span><span class="sxs-lookup"><span data-stu-id="e47b3-119">directory</span></span>|[<span data-ttu-id="e47b3-120">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="e47b3-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="e47b3-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e47b3-121">Read-only.</span></span> <span data-ttu-id="e47b3-122">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e47b3-122">Nullable.</span></span>|
|<span data-ttu-id="e47b3-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e47b3-123">deviceManagement</span></span>|[<span data-ttu-id="e47b3-124">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="e47b3-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="e47b3-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e47b3-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e47b3-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e47b3-127">JSON representation</span></span>

<span data-ttu-id="e47b3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e47b3-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
