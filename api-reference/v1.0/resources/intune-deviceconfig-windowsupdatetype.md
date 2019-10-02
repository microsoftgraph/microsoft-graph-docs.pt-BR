---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e0868516f84d15ff18a3b54c2ebfb936fb1641ed
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357126"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="5a2d1-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="5a2d1-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="5a2d1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a2d1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a2d1-105">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="5a2d1-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="5a2d1-106">Membros</span><span class="sxs-lookup"><span data-stu-id="5a2d1-106">Members</span></span>
|<span data-ttu-id="5a2d1-107">Membro</span><span class="sxs-lookup"><span data-stu-id="5a2d1-107">Member</span></span>|<span data-ttu-id="5a2d1-108">Valor</span><span class="sxs-lookup"><span data-stu-id="5a2d1-108">Value</span></span>|<span data-ttu-id="5a2d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2d1-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="5a2d1-110">userDefined</span></span>|<span data-ttu-id="5a2d1-111">,0</span><span class="sxs-lookup"><span data-stu-id="5a2d1-111">0</span></span>|<span data-ttu-id="5a2d1-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="5a2d1-112">Allow the user to set.</span></span>|
|<span data-ttu-id="5a2d1-113">todos os</span><span class="sxs-lookup"><span data-stu-id="5a2d1-113">all</span></span>|<span data-ttu-id="5a2d1-114">1</span><span class="sxs-lookup"><span data-stu-id="5a2d1-114">1</span></span>|<span data-ttu-id="5a2d1-115">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="5a2d1-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="5a2d1-116">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="5a2d1-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="5a2d1-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="5a2d1-117">businessReadyOnly</span></span>|<span data-ttu-id="5a2d1-118">duas</span><span class="sxs-lookup"><span data-stu-id="5a2d1-118">2</span></span>|<span data-ttu-id="5a2d1-119">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="5a2d1-119">Semi-annual Channel.</span></span> <span data-ttu-id="5a2d1-120">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="5a2d1-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="5a2d1-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="5a2d1-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="5a2d1-122">3D</span><span class="sxs-lookup"><span data-stu-id="5a2d1-122">3</span></span>|<span data-ttu-id="5a2d1-123">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="5a2d1-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="5a2d1-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="5a2d1-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="5a2d1-125">quatro</span><span class="sxs-lookup"><span data-stu-id="5a2d1-125">4</span></span>|<span data-ttu-id="5a2d1-126">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="5a2d1-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="5a2d1-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="5a2d1-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="5a2d1-128">0,5</span><span class="sxs-lookup"><span data-stu-id="5a2d1-128">5</span></span>|<span data-ttu-id="5a2d1-129">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="5a2d1-129">Release Windows Insider build</span></span>|




