---
title: tipo de enum androidKeyguardFeature
description: Recurso de keyguard Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429046"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="452c0-103">tipo de enum androidKeyguardFeature</span><span class="sxs-lookup"><span data-stu-id="452c0-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="452c0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="452c0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="452c0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="452c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="452c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="452c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="452c0-107">Recurso de keyguard Android.</span><span class="sxs-lookup"><span data-stu-id="452c0-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="452c0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="452c0-108">Members</span></span>
|<span data-ttu-id="452c0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="452c0-109">Member</span></span>|<span data-ttu-id="452c0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="452c0-110">Value</span></span>|<span data-ttu-id="452c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="452c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="452c0-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="452c0-112">notConfigured</span></span>|<span data-ttu-id="452c0-113">0</span><span class="sxs-lookup"><span data-stu-id="452c0-113">0</span></span>|<span data-ttu-id="452c0-114">Não configurado; Este valor será ignorado.</span><span class="sxs-lookup"><span data-stu-id="452c0-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="452c0-115">câmera</span><span class="sxs-lookup"><span data-stu-id="452c0-115">camera</span></span>|<span data-ttu-id="452c0-116">1</span><span class="sxs-lookup"><span data-stu-id="452c0-116">1</span></span>|<span data-ttu-id="452c0-117">Uso de câmera quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-118">notificações</span><span class="sxs-lookup"><span data-stu-id="452c0-118">notifications</span></span>|<span data-ttu-id="452c0-119">2</span><span class="sxs-lookup"><span data-stu-id="452c0-119">2</span></span>|<span data-ttu-id="452c0-120">Mostrando notificações quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="452c0-121">unredactedNotifications</span></span>|<span data-ttu-id="452c0-122">3</span><span class="sxs-lookup"><span data-stu-id="452c0-122">3</span></span>|<span data-ttu-id="452c0-123">Notificações de mostrando unredacted quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="452c0-124">trustAgents</span></span>|<span data-ttu-id="452c0-125">4</span><span class="sxs-lookup"><span data-stu-id="452c0-125">4</span></span>|<span data-ttu-id="452c0-126">Confie em estado do operador quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-127">impressão digital</span><span class="sxs-lookup"><span data-stu-id="452c0-127">fingerprint</span></span>|<span data-ttu-id="452c0-128">5</span><span class="sxs-lookup"><span data-stu-id="452c0-128">5</span></span>|<span data-ttu-id="452c0-129">Uso de sensor quando estiver em telas de keyguard segura de impressão digital.</span><span class="sxs-lookup"><span data-stu-id="452c0-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="452c0-130">remoteInput</span></span>|<span data-ttu-id="452c0-131">6</span><span class="sxs-lookup"><span data-stu-id="452c0-131">6</span></span>|<span data-ttu-id="452c0-132">Entrada de texto de notificação quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="452c0-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="452c0-133">allFeatures</span></span>|<span data-ttu-id="452c0-134">7</span><span class="sxs-lookup"><span data-stu-id="452c0-134">7</span></span>|<span data-ttu-id="452c0-135">Todos os recursos de keyguard quando estiver em telas de keyguard segura.</span><span class="sxs-lookup"><span data-stu-id="452c0-135">All keyguard features when on secure keyguard screens.</span></span>|




