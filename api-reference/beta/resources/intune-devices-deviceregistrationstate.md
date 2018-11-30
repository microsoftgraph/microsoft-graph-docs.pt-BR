---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
ms.openlocfilehash: 5496bce53e061894a829745fce0687815c855c01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040111"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="5d973-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="5d973-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="5d973-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d973-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d973-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d973-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d973-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5d973-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d973-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d973-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="5d973-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5d973-108">Members</span></span>
|<span data-ttu-id="5d973-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5d973-109">Member</span></span>|<span data-ttu-id="5d973-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5d973-110">Value</span></span>|<span data-ttu-id="5d973-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d973-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d973-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="5d973-112">notRegistered</span></span>|<span data-ttu-id="5d973-113">0</span><span class="sxs-lookup"><span data-stu-id="5d973-113">0</span></span>|<span data-ttu-id="5d973-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="5d973-114">The device is not registered.</span></span>|
|<span data-ttu-id="5d973-115">registrado</span><span class="sxs-lookup"><span data-stu-id="5d973-115">registered</span></span>|<span data-ttu-id="5d973-116">2</span><span class="sxs-lookup"><span data-stu-id="5d973-116">2</span></span>|<span data-ttu-id="5d973-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="5d973-117">The device is registered.</span></span>|
|<span data-ttu-id="5d973-118">revogado</span><span class="sxs-lookup"><span data-stu-id="5d973-118">revoked</span></span>|<span data-ttu-id="5d973-119">3</span><span class="sxs-lookup"><span data-stu-id="5d973-119">3</span></span>|<span data-ttu-id="5d973-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="5d973-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="5d973-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="5d973-121">keyConflict</span></span>|<span data-ttu-id="5d973-122">4</span><span class="sxs-lookup"><span data-stu-id="5d973-122">4</span></span>|<span data-ttu-id="5d973-123">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="5d973-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="5d973-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="5d973-124">approvalPending</span></span>|<span data-ttu-id="5d973-125">5</span><span class="sxs-lookup"><span data-stu-id="5d973-125">5</span></span>|<span data-ttu-id="5d973-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="5d973-126">The device is pending approval.</span></span>|
|<span data-ttu-id="5d973-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="5d973-127">certificateReset</span></span>|<span data-ttu-id="5d973-128">6</span><span class="sxs-lookup"><span data-stu-id="5d973-128">6</span></span>|<span data-ttu-id="5d973-129">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="5d973-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="5d973-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="5d973-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="5d973-131">7</span><span class="sxs-lookup"><span data-stu-id="5d973-131">7</span></span>|<span data-ttu-id="5d973-132">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="5d973-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="5d973-133">unknown</span><span class="sxs-lookup"><span data-stu-id="5d973-133">unknown</span></span>|<span data-ttu-id="5d973-134">8</span><span class="sxs-lookup"><span data-stu-id="5d973-134">8</span></span>|<span data-ttu-id="5d973-135">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5d973-135">The device registration status is unknown.</span></span>|





