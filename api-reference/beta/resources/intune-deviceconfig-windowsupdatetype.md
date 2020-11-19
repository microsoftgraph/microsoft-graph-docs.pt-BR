---
title: tipo de enumeração windowsUpdateType
description: Para quais dispositivos de filial receberão suas atualizações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01f2e14e11558d79e0e5b420eac6fd0e359a813
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272329"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="05d91-103">tipo de enumeração windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="05d91-103">windowsUpdateType enum type</span></span>

<span data-ttu-id="05d91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05d91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05d91-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="05d91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05d91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05d91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05d91-107">Para quais dispositivos de filial receberão suas atualizações</span><span class="sxs-lookup"><span data-stu-id="05d91-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="05d91-108">Membros</span><span class="sxs-lookup"><span data-stu-id="05d91-108">Members</span></span>
|<span data-ttu-id="05d91-109">Membro</span><span class="sxs-lookup"><span data-stu-id="05d91-109">Member</span></span>|<span data-ttu-id="05d91-110">Valor</span><span class="sxs-lookup"><span data-stu-id="05d91-110">Value</span></span>|<span data-ttu-id="05d91-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="05d91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05d91-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="05d91-112">userDefined</span></span>|<span data-ttu-id="05d91-113">,0</span><span class="sxs-lookup"><span data-stu-id="05d91-113">0</span></span>|<span data-ttu-id="05d91-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="05d91-114">Allow the user to set.</span></span>|
|<span data-ttu-id="05d91-115">todos os</span><span class="sxs-lookup"><span data-stu-id="05d91-115">all</span></span>|<span data-ttu-id="05d91-116">1</span><span class="sxs-lookup"><span data-stu-id="05d91-116">1</span></span>|<span data-ttu-id="05d91-117">Canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="05d91-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="05d91-118">O dispositivo obtém todas as atualizações de recursos aplicáveis do canal semestral (direcionado).</span><span class="sxs-lookup"><span data-stu-id="05d91-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="05d91-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="05d91-119">businessReadyOnly</span></span>|<span data-ttu-id="05d91-120">duas</span><span class="sxs-lookup"><span data-stu-id="05d91-120">2</span></span>|<span data-ttu-id="05d91-121">Canal semestral.</span><span class="sxs-lookup"><span data-stu-id="05d91-121">Semi-annual Channel.</span></span> <span data-ttu-id="05d91-122">O dispositivo Obtém atualizações de recursos do canal semestral.</span><span class="sxs-lookup"><span data-stu-id="05d91-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="05d91-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="05d91-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="05d91-124">3D</span><span class="sxs-lookup"><span data-stu-id="05d91-124">3</span></span>|<span data-ttu-id="05d91-125">Compilação do Windows Insider-Fast</span><span class="sxs-lookup"><span data-stu-id="05d91-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="05d91-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="05d91-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="05d91-127">4 </span><span class="sxs-lookup"><span data-stu-id="05d91-127">4</span></span>|<span data-ttu-id="05d91-128">Compilação do Windows Insider-lenta</span><span class="sxs-lookup"><span data-stu-id="05d91-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="05d91-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="05d91-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="05d91-130">5 </span><span class="sxs-lookup"><span data-stu-id="05d91-130">5</span></span>|<span data-ttu-id="05d91-131">Versão de lançamento do Windows Insider</span><span class="sxs-lookup"><span data-stu-id="05d91-131">Release Windows Insider build</span></span>|




