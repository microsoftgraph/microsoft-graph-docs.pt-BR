---
title: tipo de enumeração androidKeyguardFeature
description: Recurso de protetor de recurso Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00c63a04a2fe84f67fd9e05011eb68fce452a326
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33948559"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="71e7f-103">tipo de enumeração androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="71e7f-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="71e7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71e7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71e7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71e7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71e7f-106">Recurso de protetor de recurso Android.</span><span class="sxs-lookup"><span data-stu-id="71e7f-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="71e7f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="71e7f-107">Members</span></span>
|<span data-ttu-id="71e7f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="71e7f-108">Member</span></span>|<span data-ttu-id="71e7f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="71e7f-109">Value</span></span>|<span data-ttu-id="71e7f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71e7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71e7f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="71e7f-111">notConfigured</span></span>|<span data-ttu-id="71e7f-112">,0</span><span class="sxs-lookup"><span data-stu-id="71e7f-112">0</span></span>|<span data-ttu-id="71e7f-113">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="71e7f-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="71e7f-114">Câmara</span><span class="sxs-lookup"><span data-stu-id="71e7f-114">camera</span></span>|<span data-ttu-id="71e7f-115">1</span><span class="sxs-lookup"><span data-stu-id="71e7f-115">1</span></span>|<span data-ttu-id="71e7f-116">Uso da câmera quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="71e7f-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-117">por</span><span class="sxs-lookup"><span data-stu-id="71e7f-117">notifications</span></span>|<span data-ttu-id="71e7f-118">duas</span><span class="sxs-lookup"><span data-stu-id="71e7f-118">2</span></span>|<span data-ttu-id="71e7f-119">Mostrar notificações quando em telas do keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="71e7f-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-120">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="71e7f-120">unredactedNotifications</span></span>|<span data-ttu-id="71e7f-121">3D</span><span class="sxs-lookup"><span data-stu-id="71e7f-121">3</span></span>|<span data-ttu-id="71e7f-122">Mostrar notificações não redigidas quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="71e7f-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="71e7f-123">trustAgents</span></span>|<span data-ttu-id="71e7f-124">quatro</span><span class="sxs-lookup"><span data-stu-id="71e7f-124">4</span></span>|<span data-ttu-id="71e7f-125">Estado do agente de confiança quando em telas de proteção de segurança seguras.</span><span class="sxs-lookup"><span data-stu-id="71e7f-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-126">digitais</span><span class="sxs-lookup"><span data-stu-id="71e7f-126">fingerprint</span></span>|<span data-ttu-id="71e7f-127">0,5</span><span class="sxs-lookup"><span data-stu-id="71e7f-127">5</span></span>|<span data-ttu-id="71e7f-128">Uso do sensor de impressão digital quando estiver em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="71e7f-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="71e7f-129">remoteInput</span></span>|<span data-ttu-id="71e7f-130">6</span><span class="sxs-lookup"><span data-stu-id="71e7f-130">6</span></span>|<span data-ttu-id="71e7f-131">Entrada de texto de notificação quando em telas de keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="71e7f-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="71e7f-132">Sub-recursos</span><span class="sxs-lookup"><span data-stu-id="71e7f-132">allFeatures</span></span>|<span data-ttu-id="71e7f-133">178</span><span class="sxs-lookup"><span data-stu-id="71e7f-133">7</span></span>|<span data-ttu-id="71e7f-134">Todos os recursos de keyguard quando estão no Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="71e7f-134">All keyguard features when on secure keyguard screens.</span></span>|




