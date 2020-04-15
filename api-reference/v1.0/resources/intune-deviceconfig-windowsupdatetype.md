---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 673f95c2f1bd6e3e1d0523af91290922b793c91d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451336"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="91209-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="91209-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="91209-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91209-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91209-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91209-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91209-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="91209-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="91209-107">Membros</span><span class="sxs-lookup"><span data-stu-id="91209-107">Members</span></span>
|<span data-ttu-id="91209-108">Membro</span><span class="sxs-lookup"><span data-stu-id="91209-108">Member</span></span>|<span data-ttu-id="91209-109">Valor</span><span class="sxs-lookup"><span data-stu-id="91209-109">Value</span></span>|<span data-ttu-id="91209-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="91209-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91209-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="91209-111">userDefined</span></span>|<span data-ttu-id="91209-112">,0</span><span class="sxs-lookup"><span data-stu-id="91209-112">0</span></span>|<span data-ttu-id="91209-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="91209-113">Allow the user to set.</span></span>|
|<span data-ttu-id="91209-114">todos os</span><span class="sxs-lookup"><span data-stu-id="91209-114">all</span></span>|<span data-ttu-id="91209-115">1</span><span class="sxs-lookup"><span data-stu-id="91209-115">1</span></span>|<span data-ttu-id="91209-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="91209-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="91209-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="91209-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="91209-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="91209-118">businessReadyOnly</span></span>|<span data-ttu-id="91209-119">duas</span><span class="sxs-lookup"><span data-stu-id="91209-119">2</span></span>|<span data-ttu-id="91209-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="91209-120">Semi-annual Channel.</span></span> <span data-ttu-id="91209-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="91209-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="91209-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="91209-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="91209-123">3D</span><span class="sxs-lookup"><span data-stu-id="91209-123">3</span></span>|<span data-ttu-id="91209-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="91209-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="91209-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="91209-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="91209-126">4 </span><span class="sxs-lookup"><span data-stu-id="91209-126">4</span></span>|<span data-ttu-id="91209-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="91209-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="91209-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="91209-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="91209-129">5 </span><span class="sxs-lookup"><span data-stu-id="91209-129">5</span></span>|<span data-ttu-id="91209-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="91209-130">Release Windows Insider build</span></span>|







