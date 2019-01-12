---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d6d6b38beb34b8725587d9284dd524008320bba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961859"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="c33d6-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="c33d6-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="c33d6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c33d6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c33d6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c33d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c33d6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c33d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c33d6-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c33d6-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="c33d6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c33d6-108">Members</span></span>
|<span data-ttu-id="c33d6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c33d6-109">Member</span></span>|<span data-ttu-id="c33d6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c33d6-110">Value</span></span>|<span data-ttu-id="c33d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33d6-112">notRegistered</span><span class="sxs-lookup"><span data-stu-id="c33d6-112">notRegistered</span></span>|<span data-ttu-id="c33d6-113">0</span><span class="sxs-lookup"><span data-stu-id="c33d6-113">0</span></span>|<span data-ttu-id="c33d6-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="c33d6-114">The device is not registered.</span></span>|
|<span data-ttu-id="c33d6-115">registrado</span><span class="sxs-lookup"><span data-stu-id="c33d6-115">registered</span></span>|<span data-ttu-id="c33d6-116">2</span><span class="sxs-lookup"><span data-stu-id="c33d6-116">2</span></span>|<span data-ttu-id="c33d6-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="c33d6-117">The device is registered.</span></span>|
|<span data-ttu-id="c33d6-118">revogado</span><span class="sxs-lookup"><span data-stu-id="c33d6-118">revoked</span></span>|<span data-ttu-id="c33d6-119">3</span><span class="sxs-lookup"><span data-stu-id="c33d6-119">3</span></span>|<span data-ttu-id="c33d6-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="c33d6-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="c33d6-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="c33d6-121">keyConflict</span></span>|<span data-ttu-id="c33d6-122">4</span><span class="sxs-lookup"><span data-stu-id="c33d6-122">4</span></span>|<span data-ttu-id="c33d6-123">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="c33d6-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="c33d6-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="c33d6-124">approvalPending</span></span>|<span data-ttu-id="c33d6-125">5</span><span class="sxs-lookup"><span data-stu-id="c33d6-125">5</span></span>|<span data-ttu-id="c33d6-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="c33d6-126">The device is pending approval.</span></span>|
|<span data-ttu-id="c33d6-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="c33d6-127">certificateReset</span></span>|<span data-ttu-id="c33d6-128">6</span><span class="sxs-lookup"><span data-stu-id="c33d6-128">6</span></span>|<span data-ttu-id="c33d6-129">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="c33d6-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="c33d6-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="c33d6-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="c33d6-131">7</span><span class="sxs-lookup"><span data-stu-id="c33d6-131">7</span></span>|<span data-ttu-id="c33d6-132">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="c33d6-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="c33d6-133">unknown</span><span class="sxs-lookup"><span data-stu-id="c33d6-133">unknown</span></span>|<span data-ttu-id="c33d6-134">8</span><span class="sxs-lookup"><span data-stu-id="c33d6-134">8</span></span>|<span data-ttu-id="c33d6-135">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="c33d6-135">The device registration status is unknown.</span></span>|





