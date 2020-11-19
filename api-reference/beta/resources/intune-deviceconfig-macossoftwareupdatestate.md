---
title: tipo de enumeração macOSSoftwareUpdateState
description: Estado de atualização do software MacOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3e5f57bb4c1fce66b12084110579123d04adffc7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302877"
---
# <a name="macossoftwareupdatestate-enum-type"></a><span data-ttu-id="f6cd7-103">tipo de enumeração macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="f6cd7-103">macOSSoftwareUpdateState enum type</span></span>

<span data-ttu-id="f6cd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6cd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6cd7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6cd7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6cd7-107">Estado de atualização do software MacOS</span><span class="sxs-lookup"><span data-stu-id="f6cd7-107">MacOS Software Update State</span></span>

## <a name="members"></a><span data-ttu-id="f6cd7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f6cd7-108">Members</span></span>
|<span data-ttu-id="f6cd7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f6cd7-109">Member</span></span>|<span data-ttu-id="f6cd7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f6cd7-110">Value</span></span>|<span data-ttu-id="f6cd7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6cd7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6cd7-112">sucesso</span><span class="sxs-lookup"><span data-stu-id="f6cd7-112">success</span></span>|<span data-ttu-id="f6cd7-113">,0</span><span class="sxs-lookup"><span data-stu-id="f6cd7-113">0</span></span>|<span data-ttu-id="f6cd7-114">A atualização de software foi instalada com êxito</span><span class="sxs-lookup"><span data-stu-id="f6cd7-114">The software update successfully installed</span></span>|
|<span data-ttu-id="f6cd7-115">Baixe</span><span class="sxs-lookup"><span data-stu-id="f6cd7-115">downloading</span></span>|<span data-ttu-id="f6cd7-116">1000</span><span class="sxs-lookup"><span data-stu-id="f6cd7-116">1000</span></span>|<span data-ttu-id="f6cd7-117">A atualização de software está sendo baixada</span><span class="sxs-lookup"><span data-stu-id="f6cd7-117">The software update is being downloaded</span></span>|
|<span data-ttu-id="f6cd7-118">terminado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-118">downloaded</span></span>|<span data-ttu-id="f6cd7-119">1001</span><span class="sxs-lookup"><span data-stu-id="f6cd7-119">1001</span></span>|<span data-ttu-id="f6cd7-120">A atualização de software foi baixada</span><span class="sxs-lookup"><span data-stu-id="f6cd7-120">The software update has been downloaded</span></span>|
|<span data-ttu-id="f6cd7-121">instalado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-121">installing</span></span>|<span data-ttu-id="f6cd7-122">1002</span><span class="sxs-lookup"><span data-stu-id="f6cd7-122">1002</span></span>|<span data-ttu-id="f6cd7-123">A atualização de software está sendo instalada</span><span class="sxs-lookup"><span data-stu-id="f6cd7-123">The software update is being installed</span></span>|
|<span data-ttu-id="f6cd7-124">Estado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-124">idle</span></span>|<span data-ttu-id="f6cd7-125">1003</span><span class="sxs-lookup"><span data-stu-id="f6cd7-125">1003</span></span>|<span data-ttu-id="f6cd7-126">Nenhuma ação está sendo executada nesta atualização de software</span><span class="sxs-lookup"><span data-stu-id="f6cd7-126">No action is being taken on this software update</span></span>|
|<span data-ttu-id="f6cd7-127">disponível</span><span class="sxs-lookup"><span data-stu-id="f6cd7-127">available</span></span>|<span data-ttu-id="f6cd7-128">1004</span><span class="sxs-lookup"><span data-stu-id="f6cd7-128">1004</span></span>|<span data-ttu-id="f6cd7-129">A atualização de software está disponível no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f6cd7-129">The software update is available on the device</span></span>|
|<span data-ttu-id="f6cd7-130">agendado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-130">scheduled</span></span>|<span data-ttu-id="f6cd7-131">1005</span><span class="sxs-lookup"><span data-stu-id="f6cd7-131">1005</span></span>|<span data-ttu-id="f6cd7-132">A atualização de software foi agendada no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f6cd7-132">The software update has been scheduled on the device</span></span>|
|<span data-ttu-id="f6cd7-133">downloadFailed</span><span class="sxs-lookup"><span data-stu-id="f6cd7-133">downloadFailed</span></span>|<span data-ttu-id="f6cd7-134">2000</span><span class="sxs-lookup"><span data-stu-id="f6cd7-134">2000</span></span>|<span data-ttu-id="f6cd7-135">Falha no download da atualização de software</span><span class="sxs-lookup"><span data-stu-id="f6cd7-135">The software update download has failed</span></span>|
|<span data-ttu-id="f6cd7-136">downloadInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="f6cd7-136">downloadInsufficientSpace</span></span>|<span data-ttu-id="f6cd7-137">2001</span><span class="sxs-lookup"><span data-stu-id="f6cd7-137">2001</span></span>|<span data-ttu-id="f6cd7-138">Não há espaço suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="f6cd7-138">There is not enough space to download the update</span></span>|
|<span data-ttu-id="f6cd7-139">downloadInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="f6cd7-139">downloadInsufficientPower</span></span>|<span data-ttu-id="f6cd7-140">2002</span><span class="sxs-lookup"><span data-stu-id="f6cd7-140">2002</span></span>|<span data-ttu-id="f6cd7-141">Não há energia suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="f6cd7-141">There is not enough power to download the update</span></span>|
|<span data-ttu-id="f6cd7-142">downloadInsufficientNetwork</span><span class="sxs-lookup"><span data-stu-id="f6cd7-142">downloadInsufficientNetwork</span></span>|<span data-ttu-id="f6cd7-143">2003</span><span class="sxs-lookup"><span data-stu-id="f6cd7-143">2003</span></span>|<span data-ttu-id="f6cd7-144">Não há capacidade de rede suficiente para baixar a atualização</span><span class="sxs-lookup"><span data-stu-id="f6cd7-144">There is insufficient network capacity to download the update</span></span>|
|<span data-ttu-id="f6cd7-145">installInsufficientSpace</span><span class="sxs-lookup"><span data-stu-id="f6cd7-145">installInsufficientSpace</span></span>|<span data-ttu-id="f6cd7-146">2004</span><span class="sxs-lookup"><span data-stu-id="f6cd7-146">2004</span></span>|<span data-ttu-id="f6cd7-147">Não há espaço suficiente para instalar a atualização</span><span class="sxs-lookup"><span data-stu-id="f6cd7-147">There is not enough space to install the update</span></span>|
|<span data-ttu-id="f6cd7-148">installInsufficientPower</span><span class="sxs-lookup"><span data-stu-id="f6cd7-148">installInsufficientPower</span></span>|<span data-ttu-id="f6cd7-149">2005</span><span class="sxs-lookup"><span data-stu-id="f6cd7-149">2005</span></span>|<span data-ttu-id="f6cd7-150">Não há energia suficiente para instalar a atualização</span><span class="sxs-lookup"><span data-stu-id="f6cd7-150">There is not enough power to install the update</span></span>|
|<span data-ttu-id="f6cd7-151">installFailed</span><span class="sxs-lookup"><span data-stu-id="f6cd7-151">installFailed</span></span>|<span data-ttu-id="f6cd7-152">2006</span><span class="sxs-lookup"><span data-stu-id="f6cd7-152">2006</span></span>|<span data-ttu-id="f6cd7-153">A instalação falhou por um motivo não especificado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-153">Installation has failed for an unspecified reason</span></span>|
|<span data-ttu-id="f6cd7-154">commandFailed</span><span class="sxs-lookup"><span data-stu-id="f6cd7-154">commandFailed</span></span>|<span data-ttu-id="f6cd7-155">2007</span><span class="sxs-lookup"><span data-stu-id="f6cd7-155">2007</span></span>|<span data-ttu-id="f6cd7-156">O comando Schedule Update falhou por um motivo não especificado</span><span class="sxs-lookup"><span data-stu-id="f6cd7-156">The schedule update command has failed for an unspecified reason</span></span>|




