---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b139112db8a106dfa57c7d3ddb98e2415294914b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091373"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="6884f-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="6884f-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="6884f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6884f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6884f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6884f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6884f-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="6884f-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="6884f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6884f-107">Members</span></span>
|<span data-ttu-id="6884f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6884f-108">Member</span></span>|<span data-ttu-id="6884f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6884f-109">Value</span></span>|<span data-ttu-id="6884f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6884f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6884f-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="6884f-111">userDefined</span></span>|<span data-ttu-id="6884f-112">,0</span><span class="sxs-lookup"><span data-stu-id="6884f-112">0</span></span>|<span data-ttu-id="6884f-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="6884f-113">Allow the user to set.</span></span>|
|<span data-ttu-id="6884f-114">todos os</span><span class="sxs-lookup"><span data-stu-id="6884f-114">all</span></span>|<span data-ttu-id="6884f-115">1 </span><span class="sxs-lookup"><span data-stu-id="6884f-115">1</span></span>|<span data-ttu-id="6884f-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="6884f-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="6884f-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="6884f-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="6884f-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="6884f-118">businessReadyOnly</span></span>|<span data-ttu-id="6884f-119">2 </span><span class="sxs-lookup"><span data-stu-id="6884f-119">2</span></span>|<span data-ttu-id="6884f-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="6884f-120">Semi-annual Channel.</span></span> <span data-ttu-id="6884f-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="6884f-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="6884f-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="6884f-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="6884f-123">3D</span><span class="sxs-lookup"><span data-stu-id="6884f-123">3</span></span>|<span data-ttu-id="6884f-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="6884f-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="6884f-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="6884f-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="6884f-126">4 </span><span class="sxs-lookup"><span data-stu-id="6884f-126">4</span></span>|<span data-ttu-id="6884f-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="6884f-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="6884f-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="6884f-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="6884f-129">5 </span><span class="sxs-lookup"><span data-stu-id="6884f-129">5</span></span>|<span data-ttu-id="6884f-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="6884f-130">Release Windows Insider build</span></span>|









