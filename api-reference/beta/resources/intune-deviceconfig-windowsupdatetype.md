---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2eb02ddde8b570a6d68f077ead1123b00e82cfe0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000120"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="597e2-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="597e2-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="597e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="597e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="597e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="597e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="597e2-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="597e2-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="597e2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="597e2-107">Members</span></span>
|<span data-ttu-id="597e2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="597e2-108">Member</span></span>|<span data-ttu-id="597e2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="597e2-109">Value</span></span>|<span data-ttu-id="597e2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="597e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="597e2-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="597e2-111">userDefined</span></span>|<span data-ttu-id="597e2-112">,0</span><span class="sxs-lookup"><span data-stu-id="597e2-112">0</span></span>|<span data-ttu-id="597e2-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="597e2-113">Allow the user to set.</span></span>|
|<span data-ttu-id="597e2-114">todos os</span><span class="sxs-lookup"><span data-stu-id="597e2-114">all</span></span>|<span data-ttu-id="597e2-115">1</span><span class="sxs-lookup"><span data-stu-id="597e2-115">1</span></span>|<span data-ttu-id="597e2-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="597e2-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="597e2-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="597e2-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="597e2-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="597e2-118">businessReadyOnly</span></span>|<span data-ttu-id="597e2-119">duas</span><span class="sxs-lookup"><span data-stu-id="597e2-119">2</span></span>|<span data-ttu-id="597e2-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="597e2-120">Semi-annual Channel.</span></span> <span data-ttu-id="597e2-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="597e2-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="597e2-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="597e2-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="597e2-123">3D</span><span class="sxs-lookup"><span data-stu-id="597e2-123">3</span></span>|<span data-ttu-id="597e2-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="597e2-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="597e2-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="597e2-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="597e2-126">quatro</span><span class="sxs-lookup"><span data-stu-id="597e2-126">4</span></span>|<span data-ttu-id="597e2-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="597e2-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="597e2-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="597e2-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="597e2-129">0,5</span><span class="sxs-lookup"><span data-stu-id="597e2-129">5</span></span>|<span data-ttu-id="597e2-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="597e2-130">Release Windows Insider build</span></span>|





