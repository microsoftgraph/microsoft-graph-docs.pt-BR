---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: facd74e3ef2b2d4b6296e9b56fb99f6a2ed14fed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267408"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="bdfc8-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="bdfc8-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="bdfc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdfc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdfc8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdfc8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdfc8-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="bdfc8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bdfc8-108">Members</span></span>
|<span data-ttu-id="bdfc8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bdfc8-109">Member</span></span>|<span data-ttu-id="bdfc8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bdfc8-110">Value</span></span>|<span data-ttu-id="bdfc8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdfc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfc8-112">Não registrado</span><span class="sxs-lookup"><span data-stu-id="bdfc8-112">notRegistered</span></span>|<span data-ttu-id="bdfc8-113">,0</span><span class="sxs-lookup"><span data-stu-id="bdfc8-113">0</span></span>|<span data-ttu-id="bdfc8-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-114">The device is not registered.</span></span>|
|<span data-ttu-id="bdfc8-115">inscreve</span><span class="sxs-lookup"><span data-stu-id="bdfc8-115">registered</span></span>|<span data-ttu-id="bdfc8-116">duas</span><span class="sxs-lookup"><span data-stu-id="bdfc8-116">2</span></span>|<span data-ttu-id="bdfc8-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-117">The device is registered.</span></span>|
|<span data-ttu-id="bdfc8-118">revogado</span><span class="sxs-lookup"><span data-stu-id="bdfc8-118">revoked</span></span>|<span data-ttu-id="bdfc8-119">3D</span><span class="sxs-lookup"><span data-stu-id="bdfc8-119">3</span></span>|<span data-ttu-id="bdfc8-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="bdfc8-121">keyconflict</span><span class="sxs-lookup"><span data-stu-id="bdfc8-121">keyConflict</span></span>|<span data-ttu-id="bdfc8-122">4 </span><span class="sxs-lookup"><span data-stu-id="bdfc8-122">4</span></span>|<span data-ttu-id="bdfc8-123">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="bdfc8-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="bdfc8-124">approvalPending</span></span>|<span data-ttu-id="bdfc8-125">5 </span><span class="sxs-lookup"><span data-stu-id="bdfc8-125">5</span></span>|<span data-ttu-id="bdfc8-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-126">The device is pending approval.</span></span>|
|<span data-ttu-id="bdfc8-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="bdfc8-127">certificateReset</span></span>|<span data-ttu-id="bdfc8-128">6 </span><span class="sxs-lookup"><span data-stu-id="bdfc8-128">6</span></span>|<span data-ttu-id="bdfc8-129">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="bdfc8-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="bdfc8-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="bdfc8-131">7 </span><span class="sxs-lookup"><span data-stu-id="bdfc8-131">7</span></span>|<span data-ttu-id="bdfc8-132">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="bdfc8-133">desconhecido</span><span class="sxs-lookup"><span data-stu-id="bdfc8-133">unknown</span></span>|<span data-ttu-id="bdfc8-134">8 </span><span class="sxs-lookup"><span data-stu-id="bdfc8-134">8</span></span>|<span data-ttu-id="bdfc8-135">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="bdfc8-135">The device registration status is unknown.</span></span>|




