---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 41a6d23e42d263dd8241e960af693450ac0a7c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369504"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="45448-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="45448-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="45448-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45448-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45448-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45448-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45448-106">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="45448-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="45448-107">Membros</span><span class="sxs-lookup"><span data-stu-id="45448-107">Members</span></span>
|<span data-ttu-id="45448-108">Membro</span><span class="sxs-lookup"><span data-stu-id="45448-108">Member</span></span>|<span data-ttu-id="45448-109">Valor</span><span class="sxs-lookup"><span data-stu-id="45448-109">Value</span></span>|<span data-ttu-id="45448-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="45448-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45448-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="45448-111">userDefined</span></span>|<span data-ttu-id="45448-112">,0</span><span class="sxs-lookup"><span data-stu-id="45448-112">0</span></span>|<span data-ttu-id="45448-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="45448-113">Allow the user to set.</span></span>|
|<span data-ttu-id="45448-114">todos os</span><span class="sxs-lookup"><span data-stu-id="45448-114">all</span></span>|<span data-ttu-id="45448-115">1</span><span class="sxs-lookup"><span data-stu-id="45448-115">1</span></span>|<span data-ttu-id="45448-116">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="45448-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="45448-117">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="45448-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="45448-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="45448-118">businessReadyOnly</span></span>|<span data-ttu-id="45448-119">duas</span><span class="sxs-lookup"><span data-stu-id="45448-119">2</span></span>|<span data-ttu-id="45448-120">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="45448-120">Semi-annual Channel.</span></span> <span data-ttu-id="45448-121">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="45448-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="45448-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="45448-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="45448-123">3D</span><span class="sxs-lookup"><span data-stu-id="45448-123">3</span></span>|<span data-ttu-id="45448-124">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="45448-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="45448-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="45448-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="45448-126">quatro</span><span class="sxs-lookup"><span data-stu-id="45448-126">4</span></span>|<span data-ttu-id="45448-127">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="45448-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="45448-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="45448-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="45448-129">0,5</span><span class="sxs-lookup"><span data-stu-id="45448-129">5</span></span>|<span data-ttu-id="45448-130">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="45448-130">Release Windows Insider build</span></span>|



