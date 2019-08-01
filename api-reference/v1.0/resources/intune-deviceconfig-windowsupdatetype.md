---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7630e3cac3702380da07c2a92857d9f2786810a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027570"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f7dad-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f7dad-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="f7dad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7dad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7dad-105">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="f7dad-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="f7dad-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f7dad-106">Members</span></span>
|<span data-ttu-id="f7dad-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f7dad-107">Member</span></span>|<span data-ttu-id="f7dad-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f7dad-108">Value</span></span>|<span data-ttu-id="f7dad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7dad-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7dad-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="f7dad-110">userDefined</span></span>|<span data-ttu-id="f7dad-111">,0</span><span class="sxs-lookup"><span data-stu-id="f7dad-111">0</span></span>|<span data-ttu-id="f7dad-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="f7dad-112">Allow the user to set.</span></span>|
|<span data-ttu-id="f7dad-113">todos os</span><span class="sxs-lookup"><span data-stu-id="f7dad-113">all</span></span>|<span data-ttu-id="f7dad-114">1</span><span class="sxs-lookup"><span data-stu-id="f7dad-114">1</span></span>|<span data-ttu-id="f7dad-115">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="f7dad-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f7dad-116">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="f7dad-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f7dad-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="f7dad-117">businessReadyOnly</span></span>|<span data-ttu-id="f7dad-118">duas</span><span class="sxs-lookup"><span data-stu-id="f7dad-118">2</span></span>|<span data-ttu-id="f7dad-119">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="f7dad-119">Semi-annual Channel.</span></span> <span data-ttu-id="f7dad-120">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="f7dad-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f7dad-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="f7dad-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f7dad-122">3D</span><span class="sxs-lookup"><span data-stu-id="f7dad-122">3</span></span>|<span data-ttu-id="f7dad-123">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="f7dad-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f7dad-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="f7dad-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f7dad-125">quatro</span><span class="sxs-lookup"><span data-stu-id="f7dad-125">4</span></span>|<span data-ttu-id="f7dad-126">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="f7dad-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f7dad-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="f7dad-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f7dad-128">0,5</span><span class="sxs-lookup"><span data-stu-id="f7dad-128">5</span></span>|<span data-ttu-id="f7dad-129">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="f7dad-129">Release Windows Insider build</span></span>|



