---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7e522159df19040fcc4da3870e76b7971c95c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470675"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="f3e41-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="f3e41-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="f3e41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3e41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3e41-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3e41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3e41-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3e41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3e41-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3e41-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="f3e41-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f3e41-108">Members</span></span>
|<span data-ttu-id="f3e41-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f3e41-109">Member</span></span>|<span data-ttu-id="f3e41-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f3e41-110">Value</span></span>|<span data-ttu-id="f3e41-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3e41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3e41-112">Não registrado</span><span class="sxs-lookup"><span data-stu-id="f3e41-112">notRegistered</span></span>|<span data-ttu-id="f3e41-113">,0</span><span class="sxs-lookup"><span data-stu-id="f3e41-113">0</span></span>|<span data-ttu-id="f3e41-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="f3e41-114">The device is not registered.</span></span>|
|<span data-ttu-id="f3e41-115">inscreve</span><span class="sxs-lookup"><span data-stu-id="f3e41-115">registered</span></span>|<span data-ttu-id="f3e41-116">duas</span><span class="sxs-lookup"><span data-stu-id="f3e41-116">2</span></span>|<span data-ttu-id="f3e41-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="f3e41-117">The device is registered.</span></span>|
|<span data-ttu-id="f3e41-118">revogado</span><span class="sxs-lookup"><span data-stu-id="f3e41-118">revoked</span></span>|<span data-ttu-id="f3e41-119">3D</span><span class="sxs-lookup"><span data-stu-id="f3e41-119">3</span></span>|<span data-ttu-id="f3e41-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="f3e41-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="f3e41-121">keyconflict</span><span class="sxs-lookup"><span data-stu-id="f3e41-121">keyConflict</span></span>|<span data-ttu-id="f3e41-122">4 </span><span class="sxs-lookup"><span data-stu-id="f3e41-122">4</span></span>|<span data-ttu-id="f3e41-123">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="f3e41-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="f3e41-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="f3e41-124">approvalPending</span></span>|<span data-ttu-id="f3e41-125">5 </span><span class="sxs-lookup"><span data-stu-id="f3e41-125">5</span></span>|<span data-ttu-id="f3e41-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="f3e41-126">The device is pending approval.</span></span>|
|<span data-ttu-id="f3e41-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="f3e41-127">certificateReset</span></span>|<span data-ttu-id="f3e41-128">6 </span><span class="sxs-lookup"><span data-stu-id="f3e41-128">6</span></span>|<span data-ttu-id="f3e41-129">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="f3e41-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="f3e41-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="f3e41-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="f3e41-131">7 </span><span class="sxs-lookup"><span data-stu-id="f3e41-131">7</span></span>|<span data-ttu-id="f3e41-132">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="f3e41-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="f3e41-133">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f3e41-133">unknown</span></span>|<span data-ttu-id="f3e41-134">8 </span><span class="sxs-lookup"><span data-stu-id="f3e41-134">8</span></span>|<span data-ttu-id="f3e41-135">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="f3e41-135">The device registration status is unknown.</span></span>|



