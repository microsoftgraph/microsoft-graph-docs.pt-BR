---
title: Controle de acesso baseado em função no Microsoft Intune
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que definem e gerenciam o controle de acesso baseado em função (RBAC) para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: d72dfbf7a4051a9b98951beb8f2b25300f26122f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467708"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="738f3-103">Controle de acesso baseado em função no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="738f3-103">Role-based access control in Microsoft Intune</span></span>

<span data-ttu-id="738f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="738f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="738f3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="738f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="738f3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="738f3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="738f3-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="738f3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="738f3-108">O controle de acesso baseado em função do Intune determina quem pode executar ações em objetos do Intune e fazer alterações para aplicativos gerenciados, usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="738f3-108">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="738f3-109">Os seguintes recursos do Graph estão disponíveis para gerenciar o controle de acesso baseado em função no Intune:</span><span class="sxs-lookup"><span data-stu-id="738f3-109">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="738f3-110">Detalhes de função atribuídos ao gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="738f3-110">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="738f3-111">Atribuição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="738f3-111">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="738f3-112">Definição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="738f3-112">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="738f3-113">Vários aplicativos RBAC</span><span class="sxs-lookup"><span data-stu-id="738f3-113">Rbac application multiple</span></span>](intune-rbac-rbacapplicationmultiple.md)
- [<span data-ttu-id="738f3-114">Ação de recurso</span><span class="sxs-lookup"><span data-stu-id="738f3-114">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="738f3-115">Operação de recurso</span><span class="sxs-lookup"><span data-stu-id="738f3-115">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="738f3-116">Atribuição de função</span><span class="sxs-lookup"><span data-stu-id="738f3-116">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="738f3-117">Tipo de escopo de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="738f3-117">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="738f3-118">Definição de função</span><span class="sxs-lookup"><span data-stu-id="738f3-118">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="738f3-119">Gerenciamento de função</span><span class="sxs-lookup"><span data-stu-id="738f3-119">Role management</span></span>](intune-rbac-rolemanagement.md)
- [<span data-ttu-id="738f3-120">Permissão de função</span><span class="sxs-lookup"><span data-stu-id="738f3-120">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="738f3-121">Marca de escopo de função</span><span class="sxs-lookup"><span data-stu-id="738f3-121">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="738f3-122">Atribuição automática de marca de escopo de função</span><span class="sxs-lookup"><span data-stu-id="738f3-122">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)