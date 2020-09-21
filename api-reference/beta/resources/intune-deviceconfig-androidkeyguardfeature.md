---
title: tipo de enumeração androidKeyguardFeature
description: Recurso de protetor de recurso Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7c723079cddf33ee592fc2905056a6723b24ca02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966531"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="f8141-103">tipo de enumeração androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="f8141-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="f8141-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8141-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8141-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8141-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8141-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8141-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8141-107">Recurso de protetor de recurso Android.</span><span class="sxs-lookup"><span data-stu-id="f8141-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="f8141-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f8141-108">Members</span></span>
|<span data-ttu-id="f8141-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f8141-109">Member</span></span>|<span data-ttu-id="f8141-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f8141-110">Value</span></span>|<span data-ttu-id="f8141-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8141-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8141-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f8141-112">notConfigured</span></span>|<span data-ttu-id="f8141-113">,0</span><span class="sxs-lookup"><span data-stu-id="f8141-113">0</span></span>|<span data-ttu-id="f8141-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="f8141-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="f8141-115">Câmara</span><span class="sxs-lookup"><span data-stu-id="f8141-115">camera</span></span>|<span data-ttu-id="f8141-116">1 </span><span class="sxs-lookup"><span data-stu-id="f8141-116">1</span></span>|<span data-ttu-id="f8141-117">Uso da câmera quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="f8141-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-118">por</span><span class="sxs-lookup"><span data-stu-id="f8141-118">notifications</span></span>|<span data-ttu-id="f8141-119">2 </span><span class="sxs-lookup"><span data-stu-id="f8141-119">2</span></span>|<span data-ttu-id="f8141-120">Mostrar notificações quando em telas do keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="f8141-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="f8141-121">unredactedNotifications</span></span>|<span data-ttu-id="f8141-122">3 </span><span class="sxs-lookup"><span data-stu-id="f8141-122">3</span></span>|<span data-ttu-id="f8141-123">Mostrar notificações não redigidas quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="f8141-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="f8141-124">trustAgents</span></span>|<span data-ttu-id="f8141-125">4 </span><span class="sxs-lookup"><span data-stu-id="f8141-125">4</span></span>|<span data-ttu-id="f8141-126">Estado do agente de confiança quando em telas de proteção de segurança seguras.</span><span class="sxs-lookup"><span data-stu-id="f8141-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-127">digitais</span><span class="sxs-lookup"><span data-stu-id="f8141-127">fingerprint</span></span>|<span data-ttu-id="f8141-128">5 </span><span class="sxs-lookup"><span data-stu-id="f8141-128">5</span></span>|<span data-ttu-id="f8141-129">Uso do sensor de impressão digital quando estiver em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="f8141-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="f8141-130">remoteInput</span></span>|<span data-ttu-id="f8141-131">6 </span><span class="sxs-lookup"><span data-stu-id="f8141-131">6</span></span>|<span data-ttu-id="f8141-132">Entrada de texto de notificação quando em telas de keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="f8141-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="f8141-133">Sub-recursos</span><span class="sxs-lookup"><span data-stu-id="f8141-133">allFeatures</span></span>|<span data-ttu-id="f8141-134">7 </span><span class="sxs-lookup"><span data-stu-id="f8141-134">7</span></span>|<span data-ttu-id="f8141-135">Todos os recursos de keyguard quando estão no Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="f8141-135">All keyguard features when on secure keyguard screens.</span></span>|






