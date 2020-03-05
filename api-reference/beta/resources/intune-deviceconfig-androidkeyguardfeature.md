---
title: tipo de enumeração androidKeyguardFeature
description: Recurso de protetor de recurso Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46acc2917c8534a58221ba31f23690f84b716f81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527326"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="4e682-103">tipo de enumeração androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="4e682-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="4e682-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4e682-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e682-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e682-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e682-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e682-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e682-107">Recurso de protetor de recurso Android.</span><span class="sxs-lookup"><span data-stu-id="4e682-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="4e682-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4e682-108">Members</span></span>
|<span data-ttu-id="4e682-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4e682-109">Member</span></span>|<span data-ttu-id="4e682-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4e682-110">Value</span></span>|<span data-ttu-id="4e682-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e682-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e682-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4e682-112">notConfigured</span></span>|<span data-ttu-id="4e682-113">,0</span><span class="sxs-lookup"><span data-stu-id="4e682-113">0</span></span>|<span data-ttu-id="4e682-114">Não configurado; Esse valor é ignorado.</span><span class="sxs-lookup"><span data-stu-id="4e682-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="4e682-115">Câmara</span><span class="sxs-lookup"><span data-stu-id="4e682-115">camera</span></span>|<span data-ttu-id="4e682-116">1 </span><span class="sxs-lookup"><span data-stu-id="4e682-116">1</span></span>|<span data-ttu-id="4e682-117">Uso da câmera quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="4e682-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-118">por</span><span class="sxs-lookup"><span data-stu-id="4e682-118">notifications</span></span>|<span data-ttu-id="4e682-119">2 </span><span class="sxs-lookup"><span data-stu-id="4e682-119">2</span></span>|<span data-ttu-id="4e682-120">Mostrar notificações quando em telas do keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="4e682-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="4e682-121">unredactedNotifications</span></span>|<span data-ttu-id="4e682-122">3 </span><span class="sxs-lookup"><span data-stu-id="4e682-122">3</span></span>|<span data-ttu-id="4e682-123">Mostrar notificações não redigidas quando em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="4e682-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="4e682-124">trustAgents</span></span>|<span data-ttu-id="4e682-125">4 </span><span class="sxs-lookup"><span data-stu-id="4e682-125">4</span></span>|<span data-ttu-id="4e682-126">Estado do agente de confiança quando em telas de proteção de segurança seguras.</span><span class="sxs-lookup"><span data-stu-id="4e682-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-127">digitais</span><span class="sxs-lookup"><span data-stu-id="4e682-127">fingerprint</span></span>|<span data-ttu-id="4e682-128">5 </span><span class="sxs-lookup"><span data-stu-id="4e682-128">5</span></span>|<span data-ttu-id="4e682-129">Uso do sensor de impressão digital quando estiver em telas do Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="4e682-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="4e682-130">remoteInput</span></span>|<span data-ttu-id="4e682-131">6 </span><span class="sxs-lookup"><span data-stu-id="4e682-131">6</span></span>|<span data-ttu-id="4e682-132">Entrada de texto de notificação quando em telas de keyguard seguras.</span><span class="sxs-lookup"><span data-stu-id="4e682-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="4e682-133">Sub-recursos</span><span class="sxs-lookup"><span data-stu-id="4e682-133">allFeatures</span></span>|<span data-ttu-id="4e682-134">7 </span><span class="sxs-lookup"><span data-stu-id="4e682-134">7</span></span>|<span data-ttu-id="4e682-135">Todos os recursos de keyguard quando estão no Secure keyguard.</span><span class="sxs-lookup"><span data-stu-id="4e682-135">All keyguard features when on secure keyguard screens.</span></span>|



