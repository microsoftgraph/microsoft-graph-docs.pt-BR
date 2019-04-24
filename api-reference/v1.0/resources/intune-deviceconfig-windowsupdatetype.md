---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503594"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="bb58b-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="bb58b-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="bb58b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb58b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb58b-105">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="bb58b-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="bb58b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="bb58b-106">Members</span></span>
|<span data-ttu-id="bb58b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="bb58b-107">Member</span></span>|<span data-ttu-id="bb58b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="bb58b-108">Value</span></span>|<span data-ttu-id="bb58b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb58b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb58b-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="bb58b-110">userDefined</span></span>|<span data-ttu-id="bb58b-111">,0</span><span class="sxs-lookup"><span data-stu-id="bb58b-111">0</span></span>|<span data-ttu-id="bb58b-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="bb58b-112">Allow the user to set.</span></span>|
|<span data-ttu-id="bb58b-113">todos os</span><span class="sxs-lookup"><span data-stu-id="bb58b-113">all</span></span>|<span data-ttu-id="bb58b-114">1 </span><span class="sxs-lookup"><span data-stu-id="bb58b-114">1</span></span>|<span data-ttu-id="bb58b-115">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="bb58b-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="bb58b-116">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="bb58b-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="bb58b-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="bb58b-117">businessReadyOnly</span></span>|<span data-ttu-id="bb58b-118">2 </span><span class="sxs-lookup"><span data-stu-id="bb58b-118">2</span></span>|<span data-ttu-id="bb58b-119">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="bb58b-119">Semi-annual Channel.</span></span> <span data-ttu-id="bb58b-120">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="bb58b-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="bb58b-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="bb58b-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="bb58b-122">3 </span><span class="sxs-lookup"><span data-stu-id="bb58b-122">3</span></span>|<span data-ttu-id="bb58b-123">Compilação do Windows inSider-Fast</span><span class="sxs-lookup"><span data-stu-id="bb58b-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="bb58b-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="bb58b-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="bb58b-125">4 </span><span class="sxs-lookup"><span data-stu-id="bb58b-125">4</span></span>|<span data-ttu-id="bb58b-126">Compilação do Windows inSider-lenta</span><span class="sxs-lookup"><span data-stu-id="bb58b-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="bb58b-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="bb58b-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="bb58b-128">5 </span><span class="sxs-lookup"><span data-stu-id="bb58b-128">5</span></span>|<span data-ttu-id="bb58b-129">Versão de lançamento do Windows inSider</span><span class="sxs-lookup"><span data-stu-id="bb58b-129">Release Windows Insider build</span></span>|



