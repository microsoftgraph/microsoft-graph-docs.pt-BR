---
title: tipo de enum deviceRegistrationState
description: Status do registro do dispositivo.
ms.openlocfilehash: 9f9ee23d385ce4a7fca73e2d296c3f34063fc218
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003813"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="746a6-103">tipo de enum deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="746a6-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="746a6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="746a6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="746a6-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="746a6-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="746a6-106">Membros</span><span class="sxs-lookup"><span data-stu-id="746a6-106">Members</span></span>
|<span data-ttu-id="746a6-107">Membro</span><span class="sxs-lookup"><span data-stu-id="746a6-107">Member</span></span>|<span data-ttu-id="746a6-108">Valor</span><span class="sxs-lookup"><span data-stu-id="746a6-108">Value</span></span>|<span data-ttu-id="746a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="746a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="746a6-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="746a6-110">notRegistered</span></span>|<span data-ttu-id="746a6-111">0</span><span class="sxs-lookup"><span data-stu-id="746a6-111">0</span></span>|<span data-ttu-id="746a6-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="746a6-112">The device is not registered.</span></span>|
|<span data-ttu-id="746a6-113">registrado</span><span class="sxs-lookup"><span data-stu-id="746a6-113">registered</span></span>|<span data-ttu-id="746a6-114">2</span><span class="sxs-lookup"><span data-stu-id="746a6-114">2</span></span>|<span data-ttu-id="746a6-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="746a6-115">The device is registered.</span></span>|
|<span data-ttu-id="746a6-116">revogado</span><span class="sxs-lookup"><span data-stu-id="746a6-116">revoked</span></span>|<span data-ttu-id="746a6-117">3</span><span class="sxs-lookup"><span data-stu-id="746a6-117">3</span></span>|<span data-ttu-id="746a6-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="746a6-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="746a6-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="746a6-119">keyConflict</span></span>|<span data-ttu-id="746a6-120">4</span><span class="sxs-lookup"><span data-stu-id="746a6-120">4</span></span>|<span data-ttu-id="746a6-121">O dispositivo tem um conflito de chave.</span><span class="sxs-lookup"><span data-stu-id="746a6-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="746a6-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="746a6-122">approvalPending</span></span>|<span data-ttu-id="746a6-123">5</span><span class="sxs-lookup"><span data-stu-id="746a6-123">5</span></span>|<span data-ttu-id="746a6-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="746a6-124">The device is pending approval.</span></span>|
|<span data-ttu-id="746a6-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="746a6-125">certificateReset</span></span>|<span data-ttu-id="746a6-126">6</span><span class="sxs-lookup"><span data-stu-id="746a6-126">6</span></span>|<span data-ttu-id="746a6-127">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="746a6-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="746a6-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="746a6-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="746a6-129">7</span><span class="sxs-lookup"><span data-stu-id="746a6-129">7</span></span>|<span data-ttu-id="746a6-130">O dispositivo não está registrado e pendentes de inscrição.</span><span class="sxs-lookup"><span data-stu-id="746a6-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="746a6-131">unknown</span><span class="sxs-lookup"><span data-stu-id="746a6-131">unknown</span></span>|<span data-ttu-id="746a6-132">8</span><span class="sxs-lookup"><span data-stu-id="746a6-132">8</span></span>|<span data-ttu-id="746a6-133">O status do registro de dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="746a6-133">The device registration status is unknown.</span></span>|



