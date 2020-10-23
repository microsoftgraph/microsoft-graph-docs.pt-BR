---
title: tipo de enumeração macOSSoftwareUpdateState
description: Estado de atualização do software MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 05d2d951d8eacb93d952e20f01af6e42b30eecc1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731075"
---
# <a name="macossoftwareupdatestate-enum-type"></a><span data-ttu-id="33b35-103">tipo de enumeração macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="33b35-103">macOSSoftwareUpdateState enum type</span></span>

<span data-ttu-id="33b35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33b35-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33b35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33b35-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33b35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b35-107">Estado de atualização do software MacOS</span><span class="sxs-lookup"><span data-stu-id="33b35-107">MacOS Software Update State</span></span>

## <a name="members"></a><span data-ttu-id="33b35-108">Membros</span><span class="sxs-lookup"><span data-stu-id="33b35-108">Members</span></span>
|<span data-ttu-id="33b35-109">Membro</span><span class="sxs-lookup"><span data-stu-id="33b35-109">Member</span></span>|<span data-ttu-id="33b35-110">Valor</span><span class="sxs-lookup"><span data-stu-id="33b35-110">Value</span></span>|<span data-ttu-id="33b35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b35-112">sucesso</span><span class="sxs-lookup"><span data-stu-id="33b35-112">success</span></span>|<span data-ttu-id="33b35-113">,0</span><span class="sxs-lookup"><span data-stu-id="33b35-113">0</span></span>|<span data-ttu-id="33b35-114">A atualização de software foi instalada com êxito</span><span class="sxs-lookup"><span data-stu-id="33b35-114">The software update successfully installed</span></span>|
|<span data-ttu-id="33b35-115">Baixe</span><span class="sxs-lookup"><span data-stu-id="33b35-115">downloading</span></span>|<span data-ttu-id="33b35-116">1000</span><span class="sxs-lookup"><span data-stu-id="33b35-116">1000</span></span>|<span data-ttu-id="33b35-117">A atualização de software está sendo baixada</span><span class="sxs-lookup"><span data-stu-id="33b35-117">The software update is being downloaded</span></span>|
|<span data-ttu-id="33b35-118">terminado</span><span class="sxs-lookup"><span data-stu-id="33b35-118">downloaded</span></span>|<span data-ttu-id="33b35-119">1001</span><span class="sxs-lookup"><span data-stu-id="33b35-119">1001</span></span>|<span data-ttu-id="33b35-120">A atualização de software foi baixada</span><span class="sxs-lookup"><span data-stu-id="33b35-120">The software update has been downloaded</span></span>|
|<span data-ttu-id="33b35-121">instalado</span><span class="sxs-lookup"><span data-stu-id="33b35-121">installing</span></span>|<span data-ttu-id="33b35-122">1002</span><span class="sxs-lookup"><span data-stu-id="33b35-122">1002</span></span>|<span data-ttu-id="33b35-123">A atualização de software está sendo instalada</span><span class="sxs-lookup"><span data-stu-id="33b35-123">The software update is being installed</span></span>|
|<span data-ttu-id="33b35-124">Estado</span><span class="sxs-lookup"><span data-stu-id="33b35-124">idle</span></span>|<span data-ttu-id="33b35-125">1003</span><span class="sxs-lookup"><span data-stu-id="33b35-125">1003</span></span>|<span data-ttu-id="33b35-126">Nenhuma ação está sendo executada nesta atualização de software</span><span class="sxs-lookup"><span data-stu-id="33b35-126">No action is being taken on this software update</span></span>|
|<span data-ttu-id="33b35-127">disponível</span><span class="sxs-lookup"><span data-stu-id="33b35-127">available</span></span>|<span data-ttu-id="33b35-128">1004</span><span class="sxs-lookup"><span data-stu-id="33b35-128">1004</span></span>|<span data-ttu-id="33b35-129">A atualização de software está disponível no dispositivo</span><span class="sxs-lookup"><span data-stu-id="33b35-129">The software update is available on the device</span></span>|
|<span data-ttu-id="33b35-130">agendado</span><span class="sxs-lookup"><span data-stu-id="33b35-130">scheduled</span></span>|<span data-ttu-id="33b35-131">1005</span><span class="sxs-lookup"><span data-stu-id="33b35-131">1005</span></span>|<span data-ttu-id="33b35-132">A atualização de software foi agendada no dispositivo</span><span class="sxs-lookup"><span data-stu-id="33b35-132">The software update has been scheduled on the device</span></span>|
|<span data-ttu-id="33b35-133">downloadFailed</span><span class="sxs-lookup"><span data-stu-id="33b35-133">downloadFailed</span></span>|<span data-ttu-id="33b35-134">2000</span><span class="sxs-lookup"><span data-stu-id="33b35-134">2000</span></span>|<span data-ttu-id="33b35-135">Falha no download da atualização de software</span><span class="sxs-lookup"><span data-stu-id="33b35-135">The software update download has failed</span></span>|
|<span data-ttu-id="33b35-136">downloadInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="33b35-136">downloadInsufficientSpace</span></span>|<span data-ttu-id="33b35-137">2001</span><span class="sxs-lookup"><span data-stu-id="33b35-137">2001</span></span>|<span data-ttu-id="33b35-138">Não há espaço suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="33b35-138">There is not enough space to download the update</span></span>|
|<span data-ttu-id="33b35-139">downloadInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="33b35-139">downloadInsufficientPower</span></span>|<span data-ttu-id="33b35-140">2002</span><span class="sxs-lookup"><span data-stu-id="33b35-140">2002</span></span>|<span data-ttu-id="33b35-141">Não há energia suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="33b35-141">There is not enough power to download the update</span></span>|
|<span data-ttu-id="33b35-142">downloadInsufficientNetwork</span><span class="sxs-lookup"><span data-stu-id="33b35-142">downloadInsufficientNetwork</span></span>|<span data-ttu-id="33b35-143">2003</span><span class="sxs-lookup"><span data-stu-id="33b35-143">2003</span></span>|<span data-ttu-id="33b35-144">Não há capacidade de rede suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="33b35-144">There is insufficient network capacity to download the update</span></span>|
|<span data-ttu-id="33b35-145">installInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="33b35-145">installInsufficientSpace</span></span>|<span data-ttu-id="33b35-146">2004</span><span class="sxs-lookup"><span data-stu-id="33b35-146">2004</span></span>|<span data-ttu-id="33b35-147">Não há espaço suficiente para instalar a atualização</span><span class="sxs-lookup"><span data-stu-id="33b35-147">There is not enough space to install the update</span></span>|
|<span data-ttu-id="33b35-148">installInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="33b35-148">installInsufficientPower</span></span>|<span data-ttu-id="33b35-149">2005</span><span class="sxs-lookup"><span data-stu-id="33b35-149">2005</span></span>|<span data-ttu-id="33b35-150">Não há energia suficiente para instalar a atualização</span><span class="sxs-lookup"><span data-stu-id="33b35-150">There is not enough power to install the update</span></span>|
|<span data-ttu-id="33b35-151">installFailed</span><span class="sxs-lookup"><span data-stu-id="33b35-151">installFailed</span></span>|<span data-ttu-id="33b35-152">2006</span><span class="sxs-lookup"><span data-stu-id="33b35-152">2006</span></span>|<span data-ttu-id="33b35-153">A instalação falhou por um motivo não especificado</span><span class="sxs-lookup"><span data-stu-id="33b35-153">Installation has failed for an unspecified reason</span></span>|
|<span data-ttu-id="33b35-154">commandFailed</span><span class="sxs-lookup"><span data-stu-id="33b35-154">commandFailed</span></span>|<span data-ttu-id="33b35-155">2007</span><span class="sxs-lookup"><span data-stu-id="33b35-155">2007</span></span>|<span data-ttu-id="33b35-156">O comando Schedule Update falhou por um motivo não especificado</span><span class="sxs-lookup"><span data-stu-id="33b35-156">The schedule update command has failed for an unspecified reason</span></span>|





