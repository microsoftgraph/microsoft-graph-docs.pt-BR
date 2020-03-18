---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 851bb0a5544a807b1ae73cac15dfa5f788271703
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764093"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="4e7aa-103">tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="4e7aa-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="4e7aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e7aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7aa-106">Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="4e7aa-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4e7aa-107">Members</span></span>
|<span data-ttu-id="4e7aa-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4e7aa-108">Member</span></span>|<span data-ttu-id="4e7aa-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4e7aa-109">Value</span></span>|<span data-ttu-id="4e7aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e7aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e7aa-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="4e7aa-111">unknown</span></span>|<span data-ttu-id="4e7aa-112">,0</span><span class="sxs-lookup"><span data-stu-id="4e7aa-112">0</span></span>|<span data-ttu-id="4e7aa-113">O status da política suplementar do WindowsDefenderApplicationControl não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="4e7aa-114">sucesso</span><span class="sxs-lookup"><span data-stu-id="4e7aa-114">success</span></span>|<span data-ttu-id="4e7aa-115">1</span><span class="sxs-lookup"><span data-stu-id="4e7aa-115">1</span></span>|<span data-ttu-id="4e7aa-116">A política suplementar do WindowsDefenderApplicationControl está em vigor.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="4e7aa-117">tokenError</span><span class="sxs-lookup"><span data-stu-id="4e7aa-117">tokenError</span></span>|<span data-ttu-id="4e7aa-118">duas</span><span class="sxs-lookup"><span data-stu-id="4e7aa-118">2</span></span>|<span data-ttu-id="4e7aa-119">A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="4e7aa-120">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="4e7aa-120">notAuthorizedByToken</span></span>|<span data-ttu-id="4e7aa-121">3D</span><span class="sxs-lookup"><span data-stu-id="4e7aa-121">3</span></span>|<span data-ttu-id="4e7aa-122">O token não autoriza esta política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="4e7aa-123">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="4e7aa-123">policyNotFound</span></span>|<span data-ttu-id="4e7aa-124">4 </span><span class="sxs-lookup"><span data-stu-id="4e7aa-124">4</span></span>|<span data-ttu-id="4e7aa-125">A política suplementar do WindowsDefenderApplicationControl não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="4e7aa-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



