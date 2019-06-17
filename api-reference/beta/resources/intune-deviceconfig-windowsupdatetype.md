---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35b117b1a64650a475d392ffadf81769d3b0b08b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978665"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="65088-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="65088-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="65088-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65088-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65088-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65088-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65088-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="65088-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="65088-107">Membros</span><span class="sxs-lookup"><span data-stu-id="65088-107">Members</span></span>
|<span data-ttu-id="65088-108">Membro</span><span class="sxs-lookup"><span data-stu-id="65088-108">Member</span></span>|<span data-ttu-id="65088-109">Valor</span><span class="sxs-lookup"><span data-stu-id="65088-109">Value</span></span>|<span data-ttu-id="65088-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65088-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65088-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="65088-111">userDefined</span></span>|<span data-ttu-id="65088-112">,0</span><span class="sxs-lookup"><span data-stu-id="65088-112">0</span></span>|<span data-ttu-id="65088-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="65088-113">Allow the user to set.</span></span>|
|<span data-ttu-id="65088-114">todos os</span><span class="sxs-lookup"><span data-stu-id="65088-114">all</span></span>|<span data-ttu-id="65088-115">1</span><span class="sxs-lookup"><span data-stu-id="65088-115">1</span></span>|<span data-ttu-id="65088-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="65088-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="65088-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="65088-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="65088-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="65088-118">businessReadyOnly</span></span>|<span data-ttu-id="65088-119">duas</span><span class="sxs-lookup"><span data-stu-id="65088-119">2</span></span>|<span data-ttu-id="65088-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="65088-120">Semi-annual Channel.</span></span> <span data-ttu-id="65088-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="65088-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="65088-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="65088-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="65088-123">3D</span><span class="sxs-lookup"><span data-stu-id="65088-123">3</span></span>|<span data-ttu-id="65088-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="65088-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="65088-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="65088-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="65088-126">quatro</span><span class="sxs-lookup"><span data-stu-id="65088-126">4</span></span>|<span data-ttu-id="65088-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="65088-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="65088-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="65088-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="65088-129">0,5</span><span class="sxs-lookup"><span data-stu-id="65088-129">5</span></span>|<span data-ttu-id="65088-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="65088-130">Release Windows Insider build</span></span>|





