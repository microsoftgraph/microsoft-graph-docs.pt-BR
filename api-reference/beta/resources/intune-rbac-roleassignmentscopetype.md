---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16781d47a9db63bd346c4c33efe3cbcdd278a5e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039514"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="ce328-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="ce328-103">roleAssignmentScopeType enum type</span></span>

<span data-ttu-id="ce328-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce328-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce328-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce328-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce328-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce328-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce328-107">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ce328-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="ce328-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ce328-108">Members</span></span>
|<span data-ttu-id="ce328-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ce328-109">Member</span></span>|<span data-ttu-id="ce328-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ce328-110">Value</span></span>|<span data-ttu-id="ce328-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce328-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce328-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="ce328-112">resourceScope</span></span>|<span data-ttu-id="ce328-113">,0</span><span class="sxs-lookup"><span data-stu-id="ce328-113">0</span></span>|<span data-ttu-id="ce328-114">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="ce328-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="ce328-115">objectdevices</span><span class="sxs-lookup"><span data-stu-id="ce328-115">allDevices</span></span>|<span data-ttu-id="ce328-116">1 </span><span class="sxs-lookup"><span data-stu-id="ce328-116">1</span></span>|<span data-ttu-id="ce328-117">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="ce328-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="ce328-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="ce328-118">allLicensedUsers</span></span>|<span data-ttu-id="ce328-119">2 </span><span class="sxs-lookup"><span data-stu-id="ce328-119">2</span></span>|<span data-ttu-id="ce328-120">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="ce328-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="ce328-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="ce328-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="ce328-122">3 </span><span class="sxs-lookup"><span data-stu-id="ce328-122">3</span></span>|<span data-ttu-id="ce328-123">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="ce328-123">Allow assignments to all Intune devices and licensed users.</span></span>|






