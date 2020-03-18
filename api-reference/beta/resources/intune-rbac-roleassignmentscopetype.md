---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efdbc48a1363ba9d958c8bfe0dd2889478975083
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773249"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="dd7e4-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="dd7e4-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="dd7e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd7e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd7e4-106">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="dd7e4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="dd7e4-107">Members</span></span>
|<span data-ttu-id="dd7e4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="dd7e4-108">Member</span></span>|<span data-ttu-id="dd7e4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="dd7e4-109">Value</span></span>|<span data-ttu-id="dd7e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd7e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd7e4-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="dd7e4-111">resourceScope</span></span>|<span data-ttu-id="dd7e4-112">,0</span><span class="sxs-lookup"><span data-stu-id="dd7e4-112">0</span></span>|<span data-ttu-id="dd7e4-113">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="dd7e4-114">objectdevices</span><span class="sxs-lookup"><span data-stu-id="dd7e4-114">allDevices</span></span>|<span data-ttu-id="dd7e4-115">1</span><span class="sxs-lookup"><span data-stu-id="dd7e4-115">1</span></span>|<span data-ttu-id="dd7e4-116">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="dd7e4-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="dd7e4-117">allLicensedUsers</span></span>|<span data-ttu-id="dd7e4-118">duas</span><span class="sxs-lookup"><span data-stu-id="dd7e4-118">2</span></span>|<span data-ttu-id="dd7e4-119">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="dd7e4-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="dd7e4-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="dd7e4-121">3D</span><span class="sxs-lookup"><span data-stu-id="dd7e4-121">3</span></span>|<span data-ttu-id="dd7e4-122">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="dd7e4-122">Allow assignments to all Intune devices and licensed users.</span></span>|



