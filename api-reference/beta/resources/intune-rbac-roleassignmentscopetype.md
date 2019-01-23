---
title: tipo de enum roleAssignmentScopeType
description: Especifica o tipo de escopo para uma atribuição de função.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419888"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="9e2f9-103">tipo de enum roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="9e2f9-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="9e2f9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e2f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e2f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2f9-107">Especifica o tipo de escopo para uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="9e2f9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9e2f9-108">Members</span></span>
|<span data-ttu-id="9e2f9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9e2f9-109">Member</span></span>|<span data-ttu-id="9e2f9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9e2f9-110">Value</span></span>|<span data-ttu-id="9e2f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e2f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2f9-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="9e2f9-112">resourceScope</span></span>|<span data-ttu-id="9e2f9-113">0</span><span class="sxs-lookup"><span data-stu-id="9e2f9-113">0</span></span>|<span data-ttu-id="9e2f9-114">Permitir que as atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="9e2f9-115">allDevices</span><span class="sxs-lookup"><span data-stu-id="9e2f9-115">allDevices</span></span>|<span data-ttu-id="9e2f9-116">1</span><span class="sxs-lookup"><span data-stu-id="9e2f9-116">1</span></span>|<span data-ttu-id="9e2f9-117">Permitir que as atribuições para todos os dispositivos Intune.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="9e2f9-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9e2f9-118">allLicensedUsers</span></span>|<span data-ttu-id="9e2f9-119">2</span><span class="sxs-lookup"><span data-stu-id="9e2f9-119">2</span></span>|<span data-ttu-id="9e2f9-120">Permitir que as atribuições para todos os usuários licenciado do Intune.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="9e2f9-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9e2f9-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="9e2f9-122">3</span><span class="sxs-lookup"><span data-stu-id="9e2f9-122">3</span></span>|<span data-ttu-id="9e2f9-123">Permitir que as atribuições para todos os dispositivos de Intune e os usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="9e2f9-123">Allow assignments to all Intune devices and licensed users.</span></span>|




