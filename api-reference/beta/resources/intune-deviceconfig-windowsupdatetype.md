---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 35fe62ada736a0cd5c3a073e49851b6cad9320ab
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786148"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="10083-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="10083-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="10083-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10083-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10083-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10083-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10083-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="10083-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="10083-107">Membros</span><span class="sxs-lookup"><span data-stu-id="10083-107">Members</span></span>
|<span data-ttu-id="10083-108">Membro</span><span class="sxs-lookup"><span data-stu-id="10083-108">Member</span></span>|<span data-ttu-id="10083-109">Valor</span><span class="sxs-lookup"><span data-stu-id="10083-109">Value</span></span>|<span data-ttu-id="10083-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10083-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10083-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="10083-111">userDefined</span></span>|<span data-ttu-id="10083-112">,0</span><span class="sxs-lookup"><span data-stu-id="10083-112">0</span></span>|<span data-ttu-id="10083-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="10083-113">Allow the user to set.</span></span>|
|<span data-ttu-id="10083-114">todos os</span><span class="sxs-lookup"><span data-stu-id="10083-114">all</span></span>|<span data-ttu-id="10083-115">1</span><span class="sxs-lookup"><span data-stu-id="10083-115">1</span></span>|<span data-ttu-id="10083-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="10083-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="10083-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="10083-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="10083-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="10083-118">businessReadyOnly</span></span>|<span data-ttu-id="10083-119">duas</span><span class="sxs-lookup"><span data-stu-id="10083-119">2</span></span>|<span data-ttu-id="10083-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="10083-120">Semi-annual Channel.</span></span> <span data-ttu-id="10083-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="10083-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="10083-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="10083-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="10083-123">3D</span><span class="sxs-lookup"><span data-stu-id="10083-123">3</span></span>|<span data-ttu-id="10083-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="10083-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="10083-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="10083-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="10083-126">4 </span><span class="sxs-lookup"><span data-stu-id="10083-126">4</span></span>|<span data-ttu-id="10083-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="10083-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="10083-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="10083-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="10083-129">5 </span><span class="sxs-lookup"><span data-stu-id="10083-129">5</span></span>|<span data-ttu-id="10083-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="10083-130">Release Windows Insider build</span></span>|



