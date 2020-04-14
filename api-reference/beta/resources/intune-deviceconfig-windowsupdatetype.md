---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 77dc988570ebd089d273fd767987068313e03866
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441083"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="76398-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="76398-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="76398-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76398-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76398-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76398-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76398-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76398-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76398-107">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="76398-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="76398-108">Membros</span><span class="sxs-lookup"><span data-stu-id="76398-108">Members</span></span>
|<span data-ttu-id="76398-109">Membro</span><span class="sxs-lookup"><span data-stu-id="76398-109">Member</span></span>|<span data-ttu-id="76398-110">Valor</span><span class="sxs-lookup"><span data-stu-id="76398-110">Value</span></span>|<span data-ttu-id="76398-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76398-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76398-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="76398-112">userDefined</span></span>|<span data-ttu-id="76398-113">,0</span><span class="sxs-lookup"><span data-stu-id="76398-113">0</span></span>|<span data-ttu-id="76398-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="76398-114">Allow the user to set.</span></span>|
|<span data-ttu-id="76398-115">todos os</span><span class="sxs-lookup"><span data-stu-id="76398-115">all</span></span>|<span data-ttu-id="76398-116">1</span><span class="sxs-lookup"><span data-stu-id="76398-116">1</span></span>|<span data-ttu-id="76398-117">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="76398-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="76398-118">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="76398-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="76398-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="76398-119">businessReadyOnly</span></span>|<span data-ttu-id="76398-120">duas</span><span class="sxs-lookup"><span data-stu-id="76398-120">2</span></span>|<span data-ttu-id="76398-121">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="76398-121">Semi-annual Channel.</span></span> <span data-ttu-id="76398-122">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="76398-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="76398-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="76398-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="76398-124">3D</span><span class="sxs-lookup"><span data-stu-id="76398-124">3</span></span>|<span data-ttu-id="76398-125">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="76398-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="76398-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="76398-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="76398-127">4 </span><span class="sxs-lookup"><span data-stu-id="76398-127">4</span></span>|<span data-ttu-id="76398-128">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="76398-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="76398-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="76398-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="76398-130">5 </span><span class="sxs-lookup"><span data-stu-id="76398-130">5</span></span>|<span data-ttu-id="76398-131">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="76398-131">Release Windows Insider build</span></span>|



