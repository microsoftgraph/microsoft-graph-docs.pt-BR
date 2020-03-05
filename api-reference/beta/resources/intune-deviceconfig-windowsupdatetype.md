---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 94c82e45aae328f35b890f82755609945a9b58f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528924"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="f5852-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="f5852-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="f5852-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5852-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5852-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5852-107">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="f5852-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="f5852-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f5852-108">Members</span></span>
|<span data-ttu-id="f5852-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f5852-109">Member</span></span>|<span data-ttu-id="f5852-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f5852-110">Value</span></span>|<span data-ttu-id="f5852-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5852-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5852-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="f5852-112">userDefined</span></span>|<span data-ttu-id="f5852-113">,0</span><span class="sxs-lookup"><span data-stu-id="f5852-113">0</span></span>|<span data-ttu-id="f5852-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="f5852-114">Allow the user to set.</span></span>|
|<span data-ttu-id="f5852-115">todos os</span><span class="sxs-lookup"><span data-stu-id="f5852-115">all</span></span>|<span data-ttu-id="f5852-116">1 </span><span class="sxs-lookup"><span data-stu-id="f5852-116">1</span></span>|<span data-ttu-id="f5852-117">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="f5852-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="f5852-118">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="f5852-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="f5852-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="f5852-119">businessReadyOnly</span></span>|<span data-ttu-id="f5852-120">2 </span><span class="sxs-lookup"><span data-stu-id="f5852-120">2</span></span>|<span data-ttu-id="f5852-121">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="f5852-121">Semi-annual Channel.</span></span> <span data-ttu-id="f5852-122">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="f5852-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="f5852-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="f5852-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="f5852-124">3 </span><span class="sxs-lookup"><span data-stu-id="f5852-124">3</span></span>|<span data-ttu-id="f5852-125">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="f5852-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="f5852-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="f5852-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="f5852-127">4 </span><span class="sxs-lookup"><span data-stu-id="f5852-127">4</span></span>|<span data-ttu-id="f5852-128">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="f5852-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="f5852-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="f5852-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="f5852-130">5 </span><span class="sxs-lookup"><span data-stu-id="f5852-130">5</span></span>|<span data-ttu-id="f5852-131">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="f5852-131">Release Windows Insider build</span></span>|



