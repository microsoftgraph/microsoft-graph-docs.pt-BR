---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580971"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="fb449-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="fb449-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="fb449-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb449-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb449-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb449-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="fb449-106">Membros</span><span class="sxs-lookup"><span data-stu-id="fb449-106">Members</span></span>
|<span data-ttu-id="fb449-107">Membro</span><span class="sxs-lookup"><span data-stu-id="fb449-107">Member</span></span>|<span data-ttu-id="fb449-108">Valor</span><span class="sxs-lookup"><span data-stu-id="fb449-108">Value</span></span>|<span data-ttu-id="fb449-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb449-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb449-110">Não registrado</span><span class="sxs-lookup"><span data-stu-id="fb449-110">notRegistered</span></span>|<span data-ttu-id="fb449-111">,0</span><span class="sxs-lookup"><span data-stu-id="fb449-111">0</span></span>|<span data-ttu-id="fb449-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="fb449-112">The device is not registered.</span></span>|
|<span data-ttu-id="fb449-113">inscreve</span><span class="sxs-lookup"><span data-stu-id="fb449-113">registered</span></span>|<span data-ttu-id="fb449-114">2 </span><span class="sxs-lookup"><span data-stu-id="fb449-114">2</span></span>|<span data-ttu-id="fb449-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="fb449-115">The device is registered.</span></span>|
|<span data-ttu-id="fb449-116">revogado</span><span class="sxs-lookup"><span data-stu-id="fb449-116">revoked</span></span>|<span data-ttu-id="fb449-117">3 </span><span class="sxs-lookup"><span data-stu-id="fb449-117">3</span></span>|<span data-ttu-id="fb449-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="fb449-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="fb449-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="fb449-119">keyConflict</span></span>|<span data-ttu-id="fb449-120">4 </span><span class="sxs-lookup"><span data-stu-id="fb449-120">4</span></span>|<span data-ttu-id="fb449-121">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="fb449-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="fb449-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="fb449-122">approvalPending</span></span>|<span data-ttu-id="fb449-123">5 </span><span class="sxs-lookup"><span data-stu-id="fb449-123">5</span></span>|<span data-ttu-id="fb449-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="fb449-124">The device is pending approval.</span></span>|
|<span data-ttu-id="fb449-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="fb449-125">certificateReset</span></span>|<span data-ttu-id="fb449-126">6 </span><span class="sxs-lookup"><span data-stu-id="fb449-126">6</span></span>|<span data-ttu-id="fb449-127">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="fb449-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="fb449-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="fb449-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="fb449-129">7 </span><span class="sxs-lookup"><span data-stu-id="fb449-129">7</span></span>|<span data-ttu-id="fb449-130">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="fb449-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="fb449-131">desconhecido</span><span class="sxs-lookup"><span data-stu-id="fb449-131">unknown</span></span>|<span data-ttu-id="fb449-132">8 </span><span class="sxs-lookup"><span data-stu-id="fb449-132">8</span></span>|<span data-ttu-id="fb449-133">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="fb449-133">The device registration status is unknown.</span></span>|



