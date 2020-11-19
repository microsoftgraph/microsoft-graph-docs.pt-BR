---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3205b3ffb451f6ab62e7573e94a4347491a0c7cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259134"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="61b5f-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="61b5f-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="61b5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61b5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61b5f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61b5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61b5f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61b5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b5f-107">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="61b5f-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="61b5f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="61b5f-108">Members</span></span>
|<span data-ttu-id="61b5f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="61b5f-109">Member</span></span>|<span data-ttu-id="61b5f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="61b5f-110">Value</span></span>|<span data-ttu-id="61b5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61b5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b5f-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="61b5f-112">resourceScope</span></span>|<span data-ttu-id="61b5f-113">,0</span><span class="sxs-lookup"><span data-stu-id="61b5f-113">0</span></span>|<span data-ttu-id="61b5f-114">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="61b5f-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="61b5f-115">objectdevices</span><span class="sxs-lookup"><span data-stu-id="61b5f-115">allDevices</span></span>|<span data-ttu-id="61b5f-116">1</span><span class="sxs-lookup"><span data-stu-id="61b5f-116">1</span></span>|<span data-ttu-id="61b5f-117">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="61b5f-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="61b5f-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="61b5f-118">allLicensedUsers</span></span>|<span data-ttu-id="61b5f-119">duas</span><span class="sxs-lookup"><span data-stu-id="61b5f-119">2</span></span>|<span data-ttu-id="61b5f-120">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="61b5f-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="61b5f-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="61b5f-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="61b5f-122">3D</span><span class="sxs-lookup"><span data-stu-id="61b5f-122">3</span></span>|<span data-ttu-id="61b5f-123">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="61b5f-123">Allow assignments to all Intune devices and licensed users.</span></span>|




