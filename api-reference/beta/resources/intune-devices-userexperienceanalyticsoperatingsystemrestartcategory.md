---
title: tipo de enumeração userExperienceAnalyticsOperatingSystemRestartCategory
description: Categoria de reinicialização do sistema operacional
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 69cac1316054a7822cb169eb4070a8787c101032
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697634"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a><span data-ttu-id="5274a-103">tipo de enumeração userExperienceAnalyticsOperatingSystemRestartCategory</span><span class="sxs-lookup"><span data-stu-id="5274a-103">userExperienceAnalyticsOperatingSystemRestartCategory enum type</span></span>

<span data-ttu-id="5274a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5274a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5274a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5274a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5274a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5274a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5274a-107">Categoria de reinicialização do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5274a-107">Operating System restart category</span></span>

## <a name="members"></a><span data-ttu-id="5274a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5274a-108">Members</span></span>
|<span data-ttu-id="5274a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5274a-109">Member</span></span>|<span data-ttu-id="5274a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5274a-110">Value</span></span>|<span data-ttu-id="5274a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5274a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5274a-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5274a-112">unknown</span></span>|<span data-ttu-id="5274a-113">,0</span><span class="sxs-lookup"><span data-stu-id="5274a-113">0</span></span>|<span data-ttu-id="5274a-114">Desconhecido</span><span class="sxs-lookup"><span data-stu-id="5274a-114">Unknown</span></span>|
|<span data-ttu-id="5274a-115">restartWithUpdate</span><span class="sxs-lookup"><span data-stu-id="5274a-115">restartWithUpdate</span></span>|<span data-ttu-id="5274a-116">1</span><span class="sxs-lookup"><span data-stu-id="5274a-116">1</span></span>|<span data-ttu-id="5274a-117">Reiniciar com atualização</span><span class="sxs-lookup"><span data-stu-id="5274a-117">Restart with update</span></span>|
|<span data-ttu-id="5274a-118">restartWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="5274a-118">restartWithoutUpdate</span></span>|<span data-ttu-id="5274a-119">duas</span><span class="sxs-lookup"><span data-stu-id="5274a-119">2</span></span>|<span data-ttu-id="5274a-120">Reiniciar sem Atualizar</span><span class="sxs-lookup"><span data-stu-id="5274a-120">Restart without update</span></span>|
|<span data-ttu-id="5274a-121">blueScreen</span><span class="sxs-lookup"><span data-stu-id="5274a-121">blueScreen</span></span>|<span data-ttu-id="5274a-122">3D</span><span class="sxs-lookup"><span data-stu-id="5274a-122">3</span></span>|<span data-ttu-id="5274a-123">Reinicialização de tela azul</span><span class="sxs-lookup"><span data-stu-id="5274a-123">Blue screen restart</span></span>|
|<span data-ttu-id="5274a-124">shutdownWithUpdate</span><span class="sxs-lookup"><span data-stu-id="5274a-124">shutdownWithUpdate</span></span>|<span data-ttu-id="5274a-125">4 </span><span class="sxs-lookup"><span data-stu-id="5274a-125">4</span></span>|<span data-ttu-id="5274a-126">Desligar com atualização</span><span class="sxs-lookup"><span data-stu-id="5274a-126">Shutdown with update</span></span>|
|<span data-ttu-id="5274a-127">shutdownWithoutUpdate</span><span class="sxs-lookup"><span data-stu-id="5274a-127">shutdownWithoutUpdate</span></span>|<span data-ttu-id="5274a-128">5 </span><span class="sxs-lookup"><span data-stu-id="5274a-128">5</span></span>|<span data-ttu-id="5274a-129">Desligar sem atualização</span><span class="sxs-lookup"><span data-stu-id="5274a-129">Shutdown without update</span></span>|
|<span data-ttu-id="5274a-130">longPowerButtonPress</span><span class="sxs-lookup"><span data-stu-id="5274a-130">longPowerButtonPress</span></span>|<span data-ttu-id="5274a-131">6 </span><span class="sxs-lookup"><span data-stu-id="5274a-131">6</span></span>|<span data-ttu-id="5274a-132">Prensa de botão de energia longa</span><span class="sxs-lookup"><span data-stu-id="5274a-132">Long power button press</span></span>|
|<span data-ttu-id="5274a-133">bootError</span><span class="sxs-lookup"><span data-stu-id="5274a-133">bootError</span></span>|<span data-ttu-id="5274a-134">7 </span><span class="sxs-lookup"><span data-stu-id="5274a-134">7</span></span>|<span data-ttu-id="5274a-135">Erro de inicialização</span><span class="sxs-lookup"><span data-stu-id="5274a-135">Boot error</span></span>|





