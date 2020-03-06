---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df2fb50d31720e1f919c23020dd739e1c604fd70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532228"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ca9ee-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="ca9ee-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="ca9ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca9ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca9ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9ee-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="ca9ee-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="ca9ee-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ca9ee-107">Members</span></span>
|<span data-ttu-id="ca9ee-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ca9ee-108">Member</span></span>|<span data-ttu-id="ca9ee-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ca9ee-109">Value</span></span>|<span data-ttu-id="ca9ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca9ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9ee-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="ca9ee-111">userDefined</span></span>|<span data-ttu-id="ca9ee-112">,0</span><span class="sxs-lookup"><span data-stu-id="ca9ee-112">0</span></span>|<span data-ttu-id="ca9ee-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-113">Allow the user to set.</span></span>|
|<span data-ttu-id="ca9ee-114">todos os</span><span class="sxs-lookup"><span data-stu-id="ca9ee-114">all</span></span>|<span data-ttu-id="ca9ee-115">1 </span><span class="sxs-lookup"><span data-stu-id="ca9ee-115">1</span></span>|<span data-ttu-id="ca9ee-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="ca9ee-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ca9ee-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="ca9ee-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ca9ee-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="ca9ee-118">businessReadyOnly</span></span>|<span data-ttu-id="ca9ee-119">2 </span><span class="sxs-lookup"><span data-stu-id="ca9ee-119">2</span></span>|<span data-ttu-id="ca9ee-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-120">Semi-annual Channel.</span></span> <span data-ttu-id="ca9ee-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="ca9ee-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ca9ee-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="ca9ee-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ca9ee-123">3 </span><span class="sxs-lookup"><span data-stu-id="ca9ee-123">3</span></span>|<span data-ttu-id="ca9ee-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="ca9ee-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ca9ee-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="ca9ee-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ca9ee-126">4 </span><span class="sxs-lookup"><span data-stu-id="ca9ee-126">4</span></span>|<span data-ttu-id="ca9ee-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="ca9ee-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ca9ee-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="ca9ee-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ca9ee-129">5 </span><span class="sxs-lookup"><span data-stu-id="ca9ee-129">5</span></span>|<span data-ttu-id="ca9ee-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="ca9ee-130">Release Windows Insider build</span></span>|




