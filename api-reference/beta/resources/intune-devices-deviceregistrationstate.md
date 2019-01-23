---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396753"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="b4d2b-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="b4d2b-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="b4d2b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4d2b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4d2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d2b-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="b4d2b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b4d2b-108">Members</span></span>
|<span data-ttu-id="b4d2b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b4d2b-109">Member</span></span>|<span data-ttu-id="b4d2b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b4d2b-110">Value</span></span>|<span data-ttu-id="b4d2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d2b-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="b4d2b-112">notRegistered</span></span>|<span data-ttu-id="b4d2b-113">0</span><span class="sxs-lookup"><span data-stu-id="b4d2b-113">0</span></span>|<span data-ttu-id="b4d2b-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-114">The device is not registered.</span></span>|
|<span data-ttu-id="b4d2b-115">registrado</span><span class="sxs-lookup"><span data-stu-id="b4d2b-115">registered</span></span>|<span data-ttu-id="b4d2b-116">2</span><span class="sxs-lookup"><span data-stu-id="b4d2b-116">2</span></span>|<span data-ttu-id="b4d2b-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-117">The device is registered.</span></span>|
|<span data-ttu-id="b4d2b-118">revogado</span><span class="sxs-lookup"><span data-stu-id="b4d2b-118">revoked</span></span>|<span data-ttu-id="b4d2b-119">3</span><span class="sxs-lookup"><span data-stu-id="b4d2b-119">3</span></span>|<span data-ttu-id="b4d2b-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="b4d2b-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="b4d2b-121">keyConflict</span></span>|<span data-ttu-id="b4d2b-122">4</span><span class="sxs-lookup"><span data-stu-id="b4d2b-122">4</span></span>|<span data-ttu-id="b4d2b-123">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="b4d2b-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="b4d2b-124">approvalPending</span></span>|<span data-ttu-id="b4d2b-125">5</span><span class="sxs-lookup"><span data-stu-id="b4d2b-125">5</span></span>|<span data-ttu-id="b4d2b-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-126">The device is pending approval.</span></span>|
|<span data-ttu-id="b4d2b-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="b4d2b-127">certificateReset</span></span>|<span data-ttu-id="b4d2b-128">6</span><span class="sxs-lookup"><span data-stu-id="b4d2b-128">6</span></span>|<span data-ttu-id="b4d2b-129">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="b4d2b-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="b4d2b-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="b4d2b-131">7</span><span class="sxs-lookup"><span data-stu-id="b4d2b-131">7</span></span>|<span data-ttu-id="b4d2b-132">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="b4d2b-133">unknown</span><span class="sxs-lookup"><span data-stu-id="b4d2b-133">unknown</span></span>|<span data-ttu-id="b4d2b-134">8</span><span class="sxs-lookup"><span data-stu-id="b4d2b-134">8</span></span>|<span data-ttu-id="b4d2b-135">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b4d2b-135">The device registration status is unknown.</span></span>|




