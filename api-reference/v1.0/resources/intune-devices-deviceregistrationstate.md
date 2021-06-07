---
title: Tipo de número deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 39a4c68f2a688564284fc6045f61b84e72b748ab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751689"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="43c05-103">Tipo de número deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="43c05-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="43c05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43c05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43c05-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43c05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c05-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="43c05-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="43c05-107">Membros</span><span class="sxs-lookup"><span data-stu-id="43c05-107">Members</span></span>
|<span data-ttu-id="43c05-108">Membro</span><span class="sxs-lookup"><span data-stu-id="43c05-108">Member</span></span>|<span data-ttu-id="43c05-109">Valor</span><span class="sxs-lookup"><span data-stu-id="43c05-109">Value</span></span>|<span data-ttu-id="43c05-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43c05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43c05-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="43c05-111">notRegistered</span></span>|<span data-ttu-id="43c05-112">0</span><span class="sxs-lookup"><span data-stu-id="43c05-112">0</span></span>|<span data-ttu-id="43c05-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="43c05-113">The device is not registered.</span></span>|
|<span data-ttu-id="43c05-114">registered</span><span class="sxs-lookup"><span data-stu-id="43c05-114">registered</span></span>|<span data-ttu-id="43c05-115">2</span><span class="sxs-lookup"><span data-stu-id="43c05-115">2</span></span>|<span data-ttu-id="43c05-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="43c05-116">The device is registered.</span></span>|
|<span data-ttu-id="43c05-117">revogado</span><span class="sxs-lookup"><span data-stu-id="43c05-117">revoked</span></span>|<span data-ttu-id="43c05-118">3</span><span class="sxs-lookup"><span data-stu-id="43c05-118">3</span></span>|<span data-ttu-id="43c05-119">O dispositivo foi bloqueado, apagado ou retirado.</span><span class="sxs-lookup"><span data-stu-id="43c05-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="43c05-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="43c05-120">keyConflict</span></span>|<span data-ttu-id="43c05-121">4 </span><span class="sxs-lookup"><span data-stu-id="43c05-121">4</span></span>|<span data-ttu-id="43c05-122">O dispositivo tem um conflito chave.</span><span class="sxs-lookup"><span data-stu-id="43c05-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="43c05-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="43c05-123">approvalPending</span></span>|<span data-ttu-id="43c05-124">5 </span><span class="sxs-lookup"><span data-stu-id="43c05-124">5</span></span>|<span data-ttu-id="43c05-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="43c05-125">The device is pending approval.</span></span>|
|<span data-ttu-id="43c05-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="43c05-126">certificateReset</span></span>|<span data-ttu-id="43c05-127">6 </span><span class="sxs-lookup"><span data-stu-id="43c05-127">6</span></span>|<span data-ttu-id="43c05-128">O certificado do dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="43c05-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="43c05-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="43c05-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="43c05-130">7 </span><span class="sxs-lookup"><span data-stu-id="43c05-130">7</span></span>|<span data-ttu-id="43c05-131">O dispositivo não está registrado e o registro pendente.</span><span class="sxs-lookup"><span data-stu-id="43c05-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="43c05-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="43c05-132">unknown</span></span>|<span data-ttu-id="43c05-133">8 </span><span class="sxs-lookup"><span data-stu-id="43c05-133">8</span></span>|<span data-ttu-id="43c05-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="43c05-134">The device registration status is unknown.</span></span>|




