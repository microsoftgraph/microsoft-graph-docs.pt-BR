---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523592"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="d4844-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="d4844-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="d4844-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4844-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4844-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4844-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4844-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="d4844-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="d4844-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d4844-107">Members</span></span>
|<span data-ttu-id="d4844-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d4844-108">Member</span></span>|<span data-ttu-id="d4844-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d4844-109">Value</span></span>|<span data-ttu-id="d4844-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4844-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4844-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="d4844-111">userDefined</span></span>|<span data-ttu-id="d4844-112">,0</span><span class="sxs-lookup"><span data-stu-id="d4844-112">0</span></span>|<span data-ttu-id="d4844-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="d4844-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d4844-114">todos os</span><span class="sxs-lookup"><span data-stu-id="d4844-114">all</span></span>|<span data-ttu-id="d4844-115">1 </span><span class="sxs-lookup"><span data-stu-id="d4844-115">1</span></span>|<span data-ttu-id="d4844-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="d4844-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="d4844-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="d4844-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="d4844-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="d4844-118">businessReadyOnly</span></span>|<span data-ttu-id="d4844-119">2 </span><span class="sxs-lookup"><span data-stu-id="d4844-119">2</span></span>|<span data-ttu-id="d4844-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="d4844-120">Semi-annual Channel.</span></span> <span data-ttu-id="d4844-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="d4844-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="d4844-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="d4844-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="d4844-123">3 </span><span class="sxs-lookup"><span data-stu-id="d4844-123">3</span></span>|<span data-ttu-id="d4844-124">Compilação do Windows inSider-Fast</span><span class="sxs-lookup"><span data-stu-id="d4844-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="d4844-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="d4844-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="d4844-126">4 </span><span class="sxs-lookup"><span data-stu-id="d4844-126">4</span></span>|<span data-ttu-id="d4844-127">Compilação do Windows inSider-lenta</span><span class="sxs-lookup"><span data-stu-id="d4844-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="d4844-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="d4844-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="d4844-129">5 </span><span class="sxs-lookup"><span data-stu-id="d4844-129">5</span></span>|<span data-ttu-id="d4844-130">Versão de lançamento do Windows inSider</span><span class="sxs-lookup"><span data-stu-id="d4844-130">Release Windows Insider build</span></span>|





