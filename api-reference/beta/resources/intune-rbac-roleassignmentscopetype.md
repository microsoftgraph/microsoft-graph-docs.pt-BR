---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6f413733ffcbf7b3bad6f4abfe4a4bb7feb0e09
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982900"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="92c16-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="92c16-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="92c16-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92c16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92c16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92c16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92c16-106">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="92c16-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="92c16-107">Membros</span><span class="sxs-lookup"><span data-stu-id="92c16-107">Members</span></span>
|<span data-ttu-id="92c16-108">Membro</span><span class="sxs-lookup"><span data-stu-id="92c16-108">Member</span></span>|<span data-ttu-id="92c16-109">Valor</span><span class="sxs-lookup"><span data-stu-id="92c16-109">Value</span></span>|<span data-ttu-id="92c16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92c16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c16-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="92c16-111">resourceScope</span></span>|<span data-ttu-id="92c16-112">,0</span><span class="sxs-lookup"><span data-stu-id="92c16-112">0</span></span>|<span data-ttu-id="92c16-113">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="92c16-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="92c16-114">objectdevices</span><span class="sxs-lookup"><span data-stu-id="92c16-114">allDevices</span></span>|<span data-ttu-id="92c16-115">1</span><span class="sxs-lookup"><span data-stu-id="92c16-115">1</span></span>|<span data-ttu-id="92c16-116">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="92c16-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="92c16-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="92c16-117">allLicensedUsers</span></span>|<span data-ttu-id="92c16-118">duas</span><span class="sxs-lookup"><span data-stu-id="92c16-118">2</span></span>|<span data-ttu-id="92c16-119">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="92c16-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="92c16-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="92c16-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="92c16-121">3D</span><span class="sxs-lookup"><span data-stu-id="92c16-121">3</span></span>|<span data-ttu-id="92c16-122">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="92c16-122">Allow assignments to all Intune devices and licensed users.</span></span>|





