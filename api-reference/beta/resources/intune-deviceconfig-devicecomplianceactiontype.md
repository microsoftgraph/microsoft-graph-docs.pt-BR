---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05f9df39c563a47fa571a4badcf789ea4ddb08b1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979526"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="c73b4-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="c73b4-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="c73b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c73b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c73b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c73b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c73b4-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="c73b4-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="c73b4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c73b4-107">Members</span></span>
|<span data-ttu-id="c73b4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c73b4-108">Member</span></span>|<span data-ttu-id="c73b4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c73b4-109">Value</span></span>|<span data-ttu-id="c73b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c73b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c73b4-111">NoAction</span><span class="sxs-lookup"><span data-stu-id="c73b4-111">noAction</span></span>|<span data-ttu-id="c73b4-112">,0</span><span class="sxs-lookup"><span data-stu-id="c73b4-112">0</span></span>|<span data-ttu-id="c73b4-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="c73b4-113">No Action</span></span>|
|<span data-ttu-id="c73b4-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="c73b4-114">notification</span></span>|<span data-ttu-id="c73b4-115">1</span><span class="sxs-lookup"><span data-stu-id="c73b4-115">1</span></span>|<span data-ttu-id="c73b4-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="c73b4-116">Send Notification</span></span>|
|<span data-ttu-id="c73b4-117">Larga</span><span class="sxs-lookup"><span data-stu-id="c73b4-117">block</span></span>|<span data-ttu-id="c73b4-118">duas</span><span class="sxs-lookup"><span data-stu-id="c73b4-118">2</span></span>|<span data-ttu-id="c73b4-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="c73b4-119">Block the device in AAD</span></span>|
|<span data-ttu-id="c73b4-120">Ative</span><span class="sxs-lookup"><span data-stu-id="c73b4-120">retire</span></span>|<span data-ttu-id="c73b4-121">3D</span><span class="sxs-lookup"><span data-stu-id="c73b4-121">3</span></span>|<span data-ttu-id="c73b4-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="c73b4-122">Retire the device</span></span>|
|<span data-ttu-id="c73b4-123">revelar</span><span class="sxs-lookup"><span data-stu-id="c73b4-123">wipe</span></span>|<span data-ttu-id="c73b4-124">quatro</span><span class="sxs-lookup"><span data-stu-id="c73b4-124">4</span></span>|<span data-ttu-id="c73b4-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="c73b4-125">Wipe the device</span></span>|
|<span data-ttu-id="c73b4-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="c73b4-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="c73b4-127">0,5</span><span class="sxs-lookup"><span data-stu-id="c73b4-127">5</span></span>|<span data-ttu-id="c73b4-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c73b4-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="c73b4-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="c73b4-129">pushNotification</span></span>|<span data-ttu-id="c73b4-130">9 </span><span class="sxs-lookup"><span data-stu-id="c73b4-130">9</span></span>|<span data-ttu-id="c73b4-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="c73b4-131">Send push notification to device</span></span>|
|<span data-ttu-id="c73b4-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="c73b4-132">remoteLock</span></span>|<span data-ttu-id="c73b4-133">10 </span><span class="sxs-lookup"><span data-stu-id="c73b4-133">10</span></span>|<span data-ttu-id="c73b4-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="c73b4-134">Remotely lock the device</span></span>|





