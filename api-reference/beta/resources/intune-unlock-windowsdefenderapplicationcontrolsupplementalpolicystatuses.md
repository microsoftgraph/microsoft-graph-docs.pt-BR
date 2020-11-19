---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a8d1ecab8f108cbf885421a760671b13075ed87b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265932"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="829fb-103">tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="829fb-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

<span data-ttu-id="829fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="829fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="829fb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="829fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="829fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="829fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="829fb-107">Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="829fb-107">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="829fb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="829fb-108">Members</span></span>
|<span data-ttu-id="829fb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="829fb-109">Member</span></span>|<span data-ttu-id="829fb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="829fb-110">Value</span></span>|<span data-ttu-id="829fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="829fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="829fb-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="829fb-112">unknown</span></span>|<span data-ttu-id="829fb-113">,0</span><span class="sxs-lookup"><span data-stu-id="829fb-113">0</span></span>|<span data-ttu-id="829fb-114">O status da política suplementar do WindowsDefenderApplicationControl não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="829fb-114">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="829fb-115">sucesso</span><span class="sxs-lookup"><span data-stu-id="829fb-115">success</span></span>|<span data-ttu-id="829fb-116">1</span><span class="sxs-lookup"><span data-stu-id="829fb-116">1</span></span>|<span data-ttu-id="829fb-117">A política suplementar do WindowsDefenderApplicationControl está em vigor.</span><span class="sxs-lookup"><span data-stu-id="829fb-117">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="829fb-118">tokenError</span><span class="sxs-lookup"><span data-stu-id="829fb-118">tokenError</span></span>|<span data-ttu-id="829fb-119">duas</span><span class="sxs-lookup"><span data-stu-id="829fb-119">2</span></span>|<span data-ttu-id="829fb-120">A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.</span><span class="sxs-lookup"><span data-stu-id="829fb-120">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="829fb-121">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="829fb-121">notAuthorizedByToken</span></span>|<span data-ttu-id="829fb-122">3D</span><span class="sxs-lookup"><span data-stu-id="829fb-122">3</span></span>|<span data-ttu-id="829fb-123">O token não autoriza esta política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="829fb-123">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="829fb-124">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="829fb-124">policyNotFound</span></span>|<span data-ttu-id="829fb-125">4 </span><span class="sxs-lookup"><span data-stu-id="829fb-125">4</span></span>|<span data-ttu-id="829fb-126">A política suplementar do WindowsDefenderApplicationControl não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="829fb-126">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|




