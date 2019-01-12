---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911893"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="8bbf1-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="8bbf1-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="8bbf1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bbf1-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="8bbf1-106">Membros</span><span class="sxs-lookup"><span data-stu-id="8bbf1-106">Members</span></span>
|<span data-ttu-id="8bbf1-107">Membro</span><span class="sxs-lookup"><span data-stu-id="8bbf1-107">Member</span></span>|<span data-ttu-id="8bbf1-108">Valor</span><span class="sxs-lookup"><span data-stu-id="8bbf1-108">Value</span></span>|<span data-ttu-id="8bbf1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bbf1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbf1-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="8bbf1-110">notRegistered</span></span>|<span data-ttu-id="8bbf1-111">0</span><span class="sxs-lookup"><span data-stu-id="8bbf1-111">0</span></span>|<span data-ttu-id="8bbf1-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-112">The device is not registered.</span></span>|
|<span data-ttu-id="8bbf1-113">registrado</span><span class="sxs-lookup"><span data-stu-id="8bbf1-113">registered</span></span>|<span data-ttu-id="8bbf1-114">2</span><span class="sxs-lookup"><span data-stu-id="8bbf1-114">2</span></span>|<span data-ttu-id="8bbf1-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-115">The device is registered.</span></span>|
|<span data-ttu-id="8bbf1-116">revogado</span><span class="sxs-lookup"><span data-stu-id="8bbf1-116">revoked</span></span>|<span data-ttu-id="8bbf1-117">3</span><span class="sxs-lookup"><span data-stu-id="8bbf1-117">3</span></span>|<span data-ttu-id="8bbf1-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="8bbf1-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="8bbf1-119">keyConflict</span></span>|<span data-ttu-id="8bbf1-120">4</span><span class="sxs-lookup"><span data-stu-id="8bbf1-120">4</span></span>|<span data-ttu-id="8bbf1-121">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="8bbf1-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="8bbf1-122">approvalPending</span></span>|<span data-ttu-id="8bbf1-123">5</span><span class="sxs-lookup"><span data-stu-id="8bbf1-123">5</span></span>|<span data-ttu-id="8bbf1-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-124">The device is pending approval.</span></span>|
|<span data-ttu-id="8bbf1-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="8bbf1-125">certificateReset</span></span>|<span data-ttu-id="8bbf1-126">6</span><span class="sxs-lookup"><span data-stu-id="8bbf1-126">6</span></span>|<span data-ttu-id="8bbf1-127">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="8bbf1-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="8bbf1-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="8bbf1-129">7</span><span class="sxs-lookup"><span data-stu-id="8bbf1-129">7</span></span>|<span data-ttu-id="8bbf1-130">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="8bbf1-131">unknown</span><span class="sxs-lookup"><span data-stu-id="8bbf1-131">unknown</span></span>|<span data-ttu-id="8bbf1-132">8</span><span class="sxs-lookup"><span data-stu-id="8bbf1-132">8</span></span>|<span data-ttu-id="8bbf1-133">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="8bbf1-133">The device registration status is unknown.</span></span>|



