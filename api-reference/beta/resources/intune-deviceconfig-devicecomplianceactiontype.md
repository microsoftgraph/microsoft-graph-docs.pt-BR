---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37caa3ca741c752a67a9f90222856b31fa4978c3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947201"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="1c81c-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="1c81c-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="1c81c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c81c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c81c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c81c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c81c-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="1c81c-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="1c81c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1c81c-107">Members</span></span>
|<span data-ttu-id="1c81c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1c81c-108">Member</span></span>|<span data-ttu-id="1c81c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1c81c-109">Value</span></span>|<span data-ttu-id="1c81c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c81c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c81c-111">NoAction</span><span class="sxs-lookup"><span data-stu-id="1c81c-111">noAction</span></span>|<span data-ttu-id="1c81c-112">,0</span><span class="sxs-lookup"><span data-stu-id="1c81c-112">0</span></span>|<span data-ttu-id="1c81c-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="1c81c-113">No Action</span></span>|
|<span data-ttu-id="1c81c-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="1c81c-114">notification</span></span>|<span data-ttu-id="1c81c-115">1</span><span class="sxs-lookup"><span data-stu-id="1c81c-115">1</span></span>|<span data-ttu-id="1c81c-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="1c81c-116">Send Notification</span></span>|
|<span data-ttu-id="1c81c-117">Larga</span><span class="sxs-lookup"><span data-stu-id="1c81c-117">block</span></span>|<span data-ttu-id="1c81c-118">duas</span><span class="sxs-lookup"><span data-stu-id="1c81c-118">2</span></span>|<span data-ttu-id="1c81c-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="1c81c-119">Block the device in AAD</span></span>|
|<span data-ttu-id="1c81c-120">Ative</span><span class="sxs-lookup"><span data-stu-id="1c81c-120">retire</span></span>|<span data-ttu-id="1c81c-121">3D</span><span class="sxs-lookup"><span data-stu-id="1c81c-121">3</span></span>|<span data-ttu-id="1c81c-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1c81c-122">Retire the device</span></span>|
|<span data-ttu-id="1c81c-123">revelar</span><span class="sxs-lookup"><span data-stu-id="1c81c-123">wipe</span></span>|<span data-ttu-id="1c81c-124">quatro</span><span class="sxs-lookup"><span data-stu-id="1c81c-124">4</span></span>|<span data-ttu-id="1c81c-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1c81c-125">Wipe the device</span></span>|
|<span data-ttu-id="1c81c-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="1c81c-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="1c81c-127">0,5</span><span class="sxs-lookup"><span data-stu-id="1c81c-127">5</span></span>|<span data-ttu-id="1c81c-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1c81c-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="1c81c-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="1c81c-129">pushNotification</span></span>|<span data-ttu-id="1c81c-130">9 </span><span class="sxs-lookup"><span data-stu-id="1c81c-130">9</span></span>|<span data-ttu-id="1c81c-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="1c81c-131">Send push notification to device</span></span>|
|<span data-ttu-id="1c81c-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="1c81c-132">remoteLock</span></span>|<span data-ttu-id="1c81c-133">10 </span><span class="sxs-lookup"><span data-stu-id="1c81c-133">10</span></span>|<span data-ttu-id="1c81c-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="1c81c-134">Remotely lock the device</span></span>|




