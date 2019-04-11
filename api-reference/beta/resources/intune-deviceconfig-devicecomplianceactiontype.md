---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772941"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="b714f-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="b714f-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="b714f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b714f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b714f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b714f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b714f-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="b714f-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="b714f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b714f-107">Members</span></span>
|<span data-ttu-id="b714f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b714f-108">Member</span></span>|<span data-ttu-id="b714f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b714f-109">Value</span></span>|<span data-ttu-id="b714f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b714f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b714f-111">noAction</span><span class="sxs-lookup"><span data-stu-id="b714f-111">noAction</span></span>|<span data-ttu-id="b714f-112">,0</span><span class="sxs-lookup"><span data-stu-id="b714f-112">0</span></span>|<span data-ttu-id="b714f-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="b714f-113">No Action</span></span>|
|<span data-ttu-id="b714f-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="b714f-114">notification</span></span>|<span data-ttu-id="b714f-115">1</span><span class="sxs-lookup"><span data-stu-id="b714f-115">1</span></span>|<span data-ttu-id="b714f-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="b714f-116">Send Notification</span></span>|
|<span data-ttu-id="b714f-117">Larga</span><span class="sxs-lookup"><span data-stu-id="b714f-117">block</span></span>|<span data-ttu-id="b714f-118">duas</span><span class="sxs-lookup"><span data-stu-id="b714f-118">2</span></span>|<span data-ttu-id="b714f-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="b714f-119">Block the device in AAD</span></span>|
|<span data-ttu-id="b714f-120">Ative</span><span class="sxs-lookup"><span data-stu-id="b714f-120">retire</span></span>|<span data-ttu-id="b714f-121">3D</span><span class="sxs-lookup"><span data-stu-id="b714f-121">3</span></span>|<span data-ttu-id="b714f-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="b714f-122">Retire the device</span></span>|
|<span data-ttu-id="b714f-123">revelar</span><span class="sxs-lookup"><span data-stu-id="b714f-123">wipe</span></span>|<span data-ttu-id="b714f-124">quatro</span><span class="sxs-lookup"><span data-stu-id="b714f-124">4</span></span>|<span data-ttu-id="b714f-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="b714f-125">Wipe the device</span></span>|
|<span data-ttu-id="b714f-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="b714f-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="b714f-127">0,5</span><span class="sxs-lookup"><span data-stu-id="b714f-127">5</span></span>|<span data-ttu-id="b714f-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b714f-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="b714f-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="b714f-129">pushNotification</span></span>|<span data-ttu-id="b714f-130">241</span><span class="sxs-lookup"><span data-stu-id="b714f-130">9</span></span>|<span data-ttu-id="b714f-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="b714f-131">Send push notification to device</span></span>|
|<span data-ttu-id="b714f-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="b714f-132">remoteLock</span></span>|<span data-ttu-id="b714f-133">254</span><span class="sxs-lookup"><span data-stu-id="b714f-133">10</span></span>|<span data-ttu-id="b714f-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="b714f-134">Remotely lock the device</span></span>|





