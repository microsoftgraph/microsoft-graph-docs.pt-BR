---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6699af01c2e2a2e03e0d5ef00cce0fb572d8c57d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369238"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="7725f-103">tipo de enumeração roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="7725f-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="7725f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7725f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7725f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7725f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7725f-106">Especifica o tipo de escopo de uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7725f-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="7725f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7725f-107">Members</span></span>
|<span data-ttu-id="7725f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7725f-108">Member</span></span>|<span data-ttu-id="7725f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7725f-109">Value</span></span>|<span data-ttu-id="7725f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7725f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7725f-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="7725f-111">resourceScope</span></span>|<span data-ttu-id="7725f-112">,0</span><span class="sxs-lookup"><span data-stu-id="7725f-112">0</span></span>|<span data-ttu-id="7725f-113">Permite atribuições para o ResourceScopes especificado.</span><span class="sxs-lookup"><span data-stu-id="7725f-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="7725f-114">objectdevices</span><span class="sxs-lookup"><span data-stu-id="7725f-114">allDevices</span></span>|<span data-ttu-id="7725f-115">1</span><span class="sxs-lookup"><span data-stu-id="7725f-115">1</span></span>|<span data-ttu-id="7725f-116">Permitir atribuições de todos os dispositivos do Intune.</span><span class="sxs-lookup"><span data-stu-id="7725f-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="7725f-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="7725f-117">allLicensedUsers</span></span>|<span data-ttu-id="7725f-118">duas</span><span class="sxs-lookup"><span data-stu-id="7725f-118">2</span></span>|<span data-ttu-id="7725f-119">Permitir atribuições a todos os usuários licenciados do Intune.</span><span class="sxs-lookup"><span data-stu-id="7725f-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="7725f-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="7725f-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="7725f-121">3D</span><span class="sxs-lookup"><span data-stu-id="7725f-121">3</span></span>|<span data-ttu-id="7725f-122">Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.</span><span class="sxs-lookup"><span data-stu-id="7725f-122">Allow assignments to all Intune devices and licensed users.</span></span>|



