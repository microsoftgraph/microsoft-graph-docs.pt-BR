---
title: tipo de enumeração androidKeyguardFeature
description: Recurso de protetor de recurso Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba0520d47a362678e8d6eb1f698eee9aad2a28c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473803"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="2583d-103">tipo de enumeração androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="2583d-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="2583d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2583d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2583d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2583d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2583d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2583d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2583d-107">Recurso de protetor de recurso Android.</span><span class="sxs-lookup"><span data-stu-id="2583d-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="2583d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2583d-108">Members</span></span>
|<span data-ttu-id="2583d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2583d-109">Member</span></span>|<span data-ttu-id="2583d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2583d-110">Value</span></span>|<span data-ttu-id="2583d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2583d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2583d-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2583d-112">notConfigured</span></span>|<span data-ttu-id="2583d-113">,0</span><span class="sxs-lookup"><span data-stu-id="2583d-113">0</span></span>|<span data-ttu-id="2583d-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="2583d-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="2583d-115">Câmara</span><span class="sxs-lookup"><span data-stu-id="2583d-115">camera</span></span>|<span data-ttu-id="2583d-116">1</span><span class="sxs-lookup"><span data-stu-id="2583d-116">1</span></span>|<span data-ttu-id="2583d-117">Uso da câmera quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="2583d-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-118">por</span><span class="sxs-lookup"><span data-stu-id="2583d-118">notifications</span></span>|<span data-ttu-id="2583d-119">duas</span><span class="sxs-lookup"><span data-stu-id="2583d-119">2</span></span>|<span data-ttu-id="2583d-120">Mostrar notificações quando em telas do keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="2583d-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="2583d-121">unredactedNotifications</span></span>|<span data-ttu-id="2583d-122">3D</span><span class="sxs-lookup"><span data-stu-id="2583d-122">3</span></span>|<span data-ttu-id="2583d-123">Mostrar notificações não redigidas quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="2583d-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="2583d-124">trustAgents</span></span>|<span data-ttu-id="2583d-125">4 </span><span class="sxs-lookup"><span data-stu-id="2583d-125">4</span></span>|<span data-ttu-id="2583d-126">Estado do agente de confiança quando em telas de proteção de segurança seguras.</span><span class="sxs-lookup"><span data-stu-id="2583d-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-127">digitais</span><span class="sxs-lookup"><span data-stu-id="2583d-127">fingerprint</span></span>|<span data-ttu-id="2583d-128">5 </span><span class="sxs-lookup"><span data-stu-id="2583d-128">5</span></span>|<span data-ttu-id="2583d-129">Uso do sensor de impressão digital quando estiver em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="2583d-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="2583d-130">remoteInput</span></span>|<span data-ttu-id="2583d-131">6 </span><span class="sxs-lookup"><span data-stu-id="2583d-131">6</span></span>|<span data-ttu-id="2583d-132">Entrada de texto de notificação quando em telas de keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="2583d-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2583d-133">Sub-recursos</span><span class="sxs-lookup"><span data-stu-id="2583d-133">allFeatures</span></span>|<span data-ttu-id="2583d-134">7 </span><span class="sxs-lookup"><span data-stu-id="2583d-134">7</span></span>|<span data-ttu-id="2583d-135">Todos os recursos de keyguard quando estão no Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="2583d-135">All keyguard features when on secure keyguard screens.</span></span>|



