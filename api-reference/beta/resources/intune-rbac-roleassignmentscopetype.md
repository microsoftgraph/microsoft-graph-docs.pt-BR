---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a5589307692f6287301722ba67e54e7df0347f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010585"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="4f771-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="4f771-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="4f771-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f771-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f771-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f771-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f771-106">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="4f771-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="4f771-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4f771-107">Members</span></span>
|<span data-ttu-id="4f771-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4f771-108">Member</span></span>|<span data-ttu-id="4f771-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4f771-109">Value</span></span>|<span data-ttu-id="4f771-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f771-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f771-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="4f771-111">resourceScope</span></span>|<span data-ttu-id="4f771-112">,0</span><span class="sxs-lookup"><span data-stu-id="4f771-112">0</span></span>|<span data-ttu-id="4f771-113">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="4f771-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="4f771-114">objectdevices</span><span class="sxs-lookup"><span data-stu-id="4f771-114">allDevices</span></span>|<span data-ttu-id="4f771-115">1</span><span class="sxs-lookup"><span data-stu-id="4f771-115">1</span></span>|<span data-ttu-id="4f771-116">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="4f771-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="4f771-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="4f771-117">allLicensedUsers</span></span>|<span data-ttu-id="4f771-118">duas</span><span class="sxs-lookup"><span data-stu-id="4f771-118">2</span></span>|<span data-ttu-id="4f771-119">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="4f771-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="4f771-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="4f771-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="4f771-121">3D</span><span class="sxs-lookup"><span data-stu-id="4f771-121">3</span></span>|<span data-ttu-id="4f771-122">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="4f771-122">Allow assignments to all Intune devices and licensed users.</span></span>|





