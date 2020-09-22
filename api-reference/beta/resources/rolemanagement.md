---
title: tipo de recurso roleManagement
description: Recurso de gerenciamento de função RBAC
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 19eb561944c3d9055f8453906bfedb92701c814f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016160"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="2f307-103">tipo de recurso roleManagement</span><span class="sxs-lookup"><span data-stu-id="2f307-103">roleManagement resource type</span></span>

<span data-ttu-id="2f307-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f307-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f307-105">Representa uma entidade de gerenciamento de função RBAC da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2f307-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="2f307-106">Fornece acesso a definições de função e atribuições de função provenientes de provedores de RBAC.</span><span class="sxs-lookup"><span data-stu-id="2f307-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="2f307-107">Os provedores de diretório atualmente (Azure AD) e deviceManagement (Intune) têm suporte.</span><span class="sxs-lookup"><span data-stu-id="2f307-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="2f307-108">Para saber mais, confira:</span><span class="sxs-lookup"><span data-stu-id="2f307-108">For more information, see:</span></span> 
* <span data-ttu-id="2f307-109">[Permissões da função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="2f307-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="2f307-110">Controle de acesso baseado em função (RBAC) com o Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2f307-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="2f307-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f307-111">Methods</span></span>

<span data-ttu-id="2f307-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2f307-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2f307-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f307-113">Properties</span></span>

<span data-ttu-id="2f307-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2f307-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="2f307-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2f307-115">Relationships</span></span>

| <span data-ttu-id="2f307-116">Relação</span><span class="sxs-lookup"><span data-stu-id="2f307-116">Relationship</span></span> | <span data-ttu-id="2f307-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f307-117">Type</span></span>        | <span data-ttu-id="2f307-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f307-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f307-119">Directory</span><span class="sxs-lookup"><span data-stu-id="2f307-119">directory</span></span>|[<span data-ttu-id="2f307-120">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="2f307-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="2f307-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f307-121">Read-only.</span></span> <span data-ttu-id="2f307-122">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f307-122">Nullable.</span></span>|
|<span data-ttu-id="2f307-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="2f307-123">deviceManagement</span></span>|[<span data-ttu-id="2f307-124">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="2f307-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="2f307-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f307-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f307-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f307-127">JSON representation</span></span>

<span data-ttu-id="2f307-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f307-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


