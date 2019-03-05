---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169157"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="c74ff-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="c74ff-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="c74ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c74ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c74ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c74ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c74ff-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="c74ff-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="c74ff-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c74ff-107">Members</span></span>
|<span data-ttu-id="c74ff-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c74ff-108">Member</span></span>|<span data-ttu-id="c74ff-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c74ff-109">Value</span></span>|<span data-ttu-id="c74ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c74ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c74ff-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="c74ff-111">userDefined</span></span>|<span data-ttu-id="c74ff-112">,0</span><span class="sxs-lookup"><span data-stu-id="c74ff-112">0</span></span>|<span data-ttu-id="c74ff-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="c74ff-113">Allow the user to set.</span></span>|
|<span data-ttu-id="c74ff-114">todos os</span><span class="sxs-lookup"><span data-stu-id="c74ff-114">all</span></span>|<span data-ttu-id="c74ff-115">1</span><span class="sxs-lookup"><span data-stu-id="c74ff-115">1</span></span>|<span data-ttu-id="c74ff-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="c74ff-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="c74ff-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="c74ff-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="c74ff-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="c74ff-118">businessReadyOnly</span></span>|<span data-ttu-id="c74ff-119">duas</span><span class="sxs-lookup"><span data-stu-id="c74ff-119">2</span></span>|<span data-ttu-id="c74ff-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="c74ff-120">Semi-annual Channel.</span></span> <span data-ttu-id="c74ff-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="c74ff-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="c74ff-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="c74ff-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="c74ff-123">3D</span><span class="sxs-lookup"><span data-stu-id="c74ff-123">3</span></span>|<span data-ttu-id="c74ff-124">Compilação do Windows inSider-Fast</span><span class="sxs-lookup"><span data-stu-id="c74ff-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="c74ff-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="c74ff-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="c74ff-126">quatro</span><span class="sxs-lookup"><span data-stu-id="c74ff-126">4</span></span>|<span data-ttu-id="c74ff-127">Compilação do Windows inSider-lenta</span><span class="sxs-lookup"><span data-stu-id="c74ff-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="c74ff-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="c74ff-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="c74ff-129">0,5</span><span class="sxs-lookup"><span data-stu-id="c74ff-129">5</span></span>|<span data-ttu-id="c74ff-130">Versão de lançamento do Windows inSider</span><span class="sxs-lookup"><span data-stu-id="c74ff-130">Release Windows Insider build</span></span>|




