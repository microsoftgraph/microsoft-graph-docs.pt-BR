---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1999c999597d152396590e3faee6d7b472189500
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537654"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a><span data-ttu-id="c1d35-103">tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="c1d35-103">windowsDefenderApplicationControlSupplementalPolicyStatuses enum type</span></span>

> <span data-ttu-id="c1d35-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1d35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1d35-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1d35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1d35-106">Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="c1d35-106">Enum values for the various WindowsDefenderApplicationControl supplemental policy deployment statuses.</span></span>

## <a name="members"></a><span data-ttu-id="c1d35-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c1d35-107">Members</span></span>
|<span data-ttu-id="c1d35-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c1d35-108">Member</span></span>|<span data-ttu-id="c1d35-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c1d35-109">Value</span></span>|<span data-ttu-id="c1d35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1d35-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d35-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c1d35-111">unknown</span></span>|<span data-ttu-id="c1d35-112">,0</span><span class="sxs-lookup"><span data-stu-id="c1d35-112">0</span></span>|<span data-ttu-id="c1d35-113">O status da política suplementar do WindowsDefenderApplicationControl não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="c1d35-113">The status of the WindowsDefenderApplicationControl supplemental policy is not known.</span></span>|
|<span data-ttu-id="c1d35-114">sucesso</span><span class="sxs-lookup"><span data-stu-id="c1d35-114">success</span></span>|<span data-ttu-id="c1d35-115">1</span><span class="sxs-lookup"><span data-stu-id="c1d35-115">1</span></span>|<span data-ttu-id="c1d35-116">A política suplementar do WindowsDefenderApplicationControl está em vigor.</span><span class="sxs-lookup"><span data-stu-id="c1d35-116">The WindowsDefenderApplicationControl supplemental policy is in effect.</span></span>|
|<span data-ttu-id="c1d35-117">tokenError</span><span class="sxs-lookup"><span data-stu-id="c1d35-117">tokenError</span></span>|<span data-ttu-id="c1d35-118">duas</span><span class="sxs-lookup"><span data-stu-id="c1d35-118">2</span></span>|<span data-ttu-id="c1d35-119">A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.</span><span class="sxs-lookup"><span data-stu-id="c1d35-119">The WindowsDefenderApplicationControl supplemental policy is structurally okay but there is an error with authorizing the token.</span></span>|
|<span data-ttu-id="c1d35-120">notAuthorizedByToken</span><span class="sxs-lookup"><span data-stu-id="c1d35-120">notAuthorizedByToken</span></span>|<span data-ttu-id="c1d35-121">3D</span><span class="sxs-lookup"><span data-stu-id="c1d35-121">3</span></span>|<span data-ttu-id="c1d35-122">O token não autoriza esta política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="c1d35-122">The token does not authorize this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="c1d35-123">policyNotFound</span><span class="sxs-lookup"><span data-stu-id="c1d35-123">policyNotFound</span></span>|<span data-ttu-id="c1d35-124">4 </span><span class="sxs-lookup"><span data-stu-id="c1d35-124">4</span></span>|<span data-ttu-id="c1d35-125">A política suplementar do WindowsDefenderApplicationControl não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="c1d35-125">The WindowsDefenderApplicationControl supplemental policy is not found.</span></span>|



