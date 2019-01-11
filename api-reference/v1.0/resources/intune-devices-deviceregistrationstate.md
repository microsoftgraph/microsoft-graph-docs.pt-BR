---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b755d213d39beb228afe603b2066b55416f14c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857320"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="62d64-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="62d64-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="62d64-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="62d64-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62d64-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62d64-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="62d64-106">Membros</span><span class="sxs-lookup"><span data-stu-id="62d64-106">Members</span></span>
|<span data-ttu-id="62d64-107">Membro</span><span class="sxs-lookup"><span data-stu-id="62d64-107">Member</span></span>|<span data-ttu-id="62d64-108">Valor</span><span class="sxs-lookup"><span data-stu-id="62d64-108">Value</span></span>|<span data-ttu-id="62d64-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62d64-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d64-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="62d64-110">notRegistered</span></span>|<span data-ttu-id="62d64-111">0</span><span class="sxs-lookup"><span data-stu-id="62d64-111">0</span></span>|<span data-ttu-id="62d64-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="62d64-112">The device is not registered.</span></span>|
|<span data-ttu-id="62d64-113">registrado</span><span class="sxs-lookup"><span data-stu-id="62d64-113">registered</span></span>|<span data-ttu-id="62d64-114">2</span><span class="sxs-lookup"><span data-stu-id="62d64-114">2</span></span>|<span data-ttu-id="62d64-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="62d64-115">The device is registered.</span></span>|
|<span data-ttu-id="62d64-116">revogado</span><span class="sxs-lookup"><span data-stu-id="62d64-116">revoked</span></span>|<span data-ttu-id="62d64-117">3</span><span class="sxs-lookup"><span data-stu-id="62d64-117">3</span></span>|<span data-ttu-id="62d64-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="62d64-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="62d64-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="62d64-119">keyConflict</span></span>|<span data-ttu-id="62d64-120">4</span><span class="sxs-lookup"><span data-stu-id="62d64-120">4</span></span>|<span data-ttu-id="62d64-121">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="62d64-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="62d64-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="62d64-122">approvalPending</span></span>|<span data-ttu-id="62d64-123">5</span><span class="sxs-lookup"><span data-stu-id="62d64-123">5</span></span>|<span data-ttu-id="62d64-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="62d64-124">The device is pending approval.</span></span>|
|<span data-ttu-id="62d64-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="62d64-125">certificateReset</span></span>|<span data-ttu-id="62d64-126">6</span><span class="sxs-lookup"><span data-stu-id="62d64-126">6</span></span>|<span data-ttu-id="62d64-127">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="62d64-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="62d64-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="62d64-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="62d64-129">7</span><span class="sxs-lookup"><span data-stu-id="62d64-129">7</span></span>|<span data-ttu-id="62d64-130">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="62d64-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="62d64-131">unknown</span><span class="sxs-lookup"><span data-stu-id="62d64-131">unknown</span></span>|<span data-ttu-id="62d64-132">8</span><span class="sxs-lookup"><span data-stu-id="62d64-132">8</span></span>|<span data-ttu-id="62d64-133">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="62d64-133">The device registration status is unknown.</span></span>|



