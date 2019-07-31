---
title: Controle de acesso baseado em função no Microsoft Intune
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que definem e gerenciam o controle de acesso baseado em função (RBAC) para uma organização de locatário.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 3f16673a2a54b4ed0de380ddd4b66aa6c74c1106
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967676"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="1d6d4-103">Controle de acesso baseado em função no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1d6d4-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="1d6d4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1d6d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d6d4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1d6d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d6d4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d6d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d6d4-107">O controle de acesso baseado em função do Intune determina quem pode executar ações em objetos do Intune e fazer alterações para aplicativos gerenciados, usuários e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1d6d4-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="1d6d4-108">Os seguintes recursos do Graph estão disponíveis para gerenciar o controle de acesso baseado em função no Intune:</span><span class="sxs-lookup"><span data-stu-id="1d6d4-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="1d6d4-109">Detalhes de função atribuídos ao gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="1d6d4-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="1d6d4-110">Atribuição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="1d6d4-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="1d6d4-111">Definição de função de gerenciamento de aplicativo e dispositivo</span><span class="sxs-lookup"><span data-stu-id="1d6d4-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="1d6d4-112">Ação de recurso</span><span class="sxs-lookup"><span data-stu-id="1d6d4-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="1d6d4-113">Operação de recurso</span><span class="sxs-lookup"><span data-stu-id="1d6d4-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="1d6d4-114">Atribuição de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="1d6d4-115">Tipo de escopo de atribuição de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="1d6d4-116">Definição de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="1d6d4-117">Permissão de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="1d6d4-118">Marca de escopo de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="1d6d4-119">Atribuição automática de marca de escopo de função</span><span class="sxs-lookup"><span data-stu-id="1d6d4-119">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)
