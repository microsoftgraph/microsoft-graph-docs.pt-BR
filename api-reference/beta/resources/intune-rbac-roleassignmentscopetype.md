---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573050"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="9a058-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="9a058-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="9a058-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a058-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a058-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a058-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a058-106">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="9a058-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="9a058-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9a058-107">Members</span></span>
|<span data-ttu-id="9a058-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9a058-108">Member</span></span>|<span data-ttu-id="9a058-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9a058-109">Value</span></span>|<span data-ttu-id="9a058-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a058-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a058-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="9a058-111">resourceScope</span></span>|<span data-ttu-id="9a058-112">,0</span><span class="sxs-lookup"><span data-stu-id="9a058-112">0</span></span>|<span data-ttu-id="9a058-113">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="9a058-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="9a058-114">objectDevices</span><span class="sxs-lookup"><span data-stu-id="9a058-114">allDevices</span></span>|<span data-ttu-id="9a058-115">1 </span><span class="sxs-lookup"><span data-stu-id="9a058-115">1</span></span>|<span data-ttu-id="9a058-116">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="9a058-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="9a058-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9a058-117">allLicensedUsers</span></span>|<span data-ttu-id="9a058-118">2 </span><span class="sxs-lookup"><span data-stu-id="9a058-118">2</span></span>|<span data-ttu-id="9a058-119">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="9a058-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="9a058-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="9a058-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="9a058-121">3 </span><span class="sxs-lookup"><span data-stu-id="9a058-121">3</span></span>|<span data-ttu-id="9a058-122">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="9a058-122">Allow assignments to all Intune devices and licensed users.</span></span>|





