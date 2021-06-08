---
title: Tipo de número windowsUpdateType
description: De quais dispositivos de filial receberão suas atualizações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f49158686884d55825751a9314a50a9ab9a16d57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759942"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="edfcc-103">Tipo de número windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="edfcc-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="edfcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edfcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edfcc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edfcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edfcc-106">De quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="edfcc-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="edfcc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="edfcc-107">Members</span></span>
|<span data-ttu-id="edfcc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="edfcc-108">Member</span></span>|<span data-ttu-id="edfcc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="edfcc-109">Value</span></span>|<span data-ttu-id="edfcc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="edfcc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfcc-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="edfcc-111">userDefined</span></span>|<span data-ttu-id="edfcc-112">0</span><span class="sxs-lookup"><span data-stu-id="edfcc-112">0</span></span>|<span data-ttu-id="edfcc-113">Permitir que o usuário desem conjunto.</span><span class="sxs-lookup"><span data-stu-id="edfcc-113">Allow the user to set.</span></span>|
|<span data-ttu-id="edfcc-114">all</span><span class="sxs-lookup"><span data-stu-id="edfcc-114">all</span></span>|<span data-ttu-id="edfcc-115">1</span><span class="sxs-lookup"><span data-stu-id="edfcc-115">1</span></span>|<span data-ttu-id="edfcc-116">Canal Semes anual (Direcionado).</span><span class="sxs-lookup"><span data-stu-id="edfcc-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="edfcc-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do Canal Semes anual (Direcionado).</span><span class="sxs-lookup"><span data-stu-id="edfcc-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="edfcc-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="edfcc-118">businessReadyOnly</span></span>|<span data-ttu-id="edfcc-119">2</span><span class="sxs-lookup"><span data-stu-id="edfcc-119">2</span></span>|<span data-ttu-id="edfcc-120">Canal Semes anual.</span><span class="sxs-lookup"><span data-stu-id="edfcc-120">Semi-annual Channel.</span></span> <span data-ttu-id="edfcc-121">O dispositivo obtém atualizações de recursos do Canal Semesanuais.</span><span class="sxs-lookup"><span data-stu-id="edfcc-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="edfcc-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="edfcc-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="edfcc-123">3</span><span class="sxs-lookup"><span data-stu-id="edfcc-123">3</span></span>|<span data-ttu-id="edfcc-124">Windows Insider build - Fast</span><span class="sxs-lookup"><span data-stu-id="edfcc-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="edfcc-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="edfcc-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="edfcc-126">4 </span><span class="sxs-lookup"><span data-stu-id="edfcc-126">4</span></span>|<span data-ttu-id="edfcc-127">Windows Insider build - Slow</span><span class="sxs-lookup"><span data-stu-id="edfcc-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="edfcc-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="edfcc-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="edfcc-129">5 </span><span class="sxs-lookup"><span data-stu-id="edfcc-129">5</span></span>|<span data-ttu-id="edfcc-130">Versão Windows build do Insider</span><span class="sxs-lookup"><span data-stu-id="edfcc-130">Release Windows Insider build</span></span>|




