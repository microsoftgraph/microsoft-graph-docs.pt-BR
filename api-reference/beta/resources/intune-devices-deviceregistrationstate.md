---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7633419ebeeb5c5865cd1a80c251effbf314b018
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829761"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="7b881-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="7b881-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="7b881-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b881-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b881-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b881-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b881-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7b881-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b881-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7b881-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="7b881-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7b881-108">Members</span></span>
|<span data-ttu-id="7b881-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7b881-109">Member</span></span>|<span data-ttu-id="7b881-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7b881-110">Value</span></span>|<span data-ttu-id="7b881-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b881-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b881-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="7b881-112">notRegistered</span></span>|<span data-ttu-id="7b881-113">0</span><span class="sxs-lookup"><span data-stu-id="7b881-113">0</span></span>|<span data-ttu-id="7b881-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="7b881-114">The device is not registered.</span></span>|
|<span data-ttu-id="7b881-115">registrado</span><span class="sxs-lookup"><span data-stu-id="7b881-115">registered</span></span>|<span data-ttu-id="7b881-116">2</span><span class="sxs-lookup"><span data-stu-id="7b881-116">2</span></span>|<span data-ttu-id="7b881-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="7b881-117">The device is registered.</span></span>|
|<span data-ttu-id="7b881-118">revogado</span><span class="sxs-lookup"><span data-stu-id="7b881-118">revoked</span></span>|<span data-ttu-id="7b881-119">3</span><span class="sxs-lookup"><span data-stu-id="7b881-119">3</span></span>|<span data-ttu-id="7b881-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="7b881-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="7b881-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="7b881-121">keyConflict</span></span>|<span data-ttu-id="7b881-122">4</span><span class="sxs-lookup"><span data-stu-id="7b881-122">4</span></span>|<span data-ttu-id="7b881-123">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="7b881-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="7b881-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="7b881-124">approvalPending</span></span>|<span data-ttu-id="7b881-125">5</span><span class="sxs-lookup"><span data-stu-id="7b881-125">5</span></span>|<span data-ttu-id="7b881-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="7b881-126">The device is pending approval.</span></span>|
|<span data-ttu-id="7b881-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="7b881-127">certificateReset</span></span>|<span data-ttu-id="7b881-128">6</span><span class="sxs-lookup"><span data-stu-id="7b881-128">6</span></span>|<span data-ttu-id="7b881-129">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="7b881-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="7b881-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="7b881-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="7b881-131">7</span><span class="sxs-lookup"><span data-stu-id="7b881-131">7</span></span>|<span data-ttu-id="7b881-132">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="7b881-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="7b881-133">unknown</span><span class="sxs-lookup"><span data-stu-id="7b881-133">unknown</span></span>|<span data-ttu-id="7b881-134">8</span><span class="sxs-lookup"><span data-stu-id="7b881-134">8</span></span>|<span data-ttu-id="7b881-135">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7b881-135">The device registration status is unknown.</span></span>|





