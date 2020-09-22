---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f441179e425f341d55eaee02525894aec53e487c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085042"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="85a3b-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="85a3b-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="85a3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85a3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85a3b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85a3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85a3b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85a3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85a3b-107">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="85a3b-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="85a3b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="85a3b-108">Members</span></span>
|<span data-ttu-id="85a3b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="85a3b-109">Member</span></span>|<span data-ttu-id="85a3b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="85a3b-110">Value</span></span>|<span data-ttu-id="85a3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85a3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85a3b-112">NoAction</span><span class="sxs-lookup"><span data-stu-id="85a3b-112">noAction</span></span>|<span data-ttu-id="85a3b-113">,0</span><span class="sxs-lookup"><span data-stu-id="85a3b-113">0</span></span>|<span data-ttu-id="85a3b-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="85a3b-114">No Action</span></span>|
|<span data-ttu-id="85a3b-115">Notifica</span><span class="sxs-lookup"><span data-stu-id="85a3b-115">notification</span></span>|<span data-ttu-id="85a3b-116">1 </span><span class="sxs-lookup"><span data-stu-id="85a3b-116">1</span></span>|<span data-ttu-id="85a3b-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="85a3b-117">Send Notification</span></span>|
|<span data-ttu-id="85a3b-118">Larga</span><span class="sxs-lookup"><span data-stu-id="85a3b-118">block</span></span>|<span data-ttu-id="85a3b-119">2 </span><span class="sxs-lookup"><span data-stu-id="85a3b-119">2</span></span>|<span data-ttu-id="85a3b-120">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="85a3b-120">Block the device in AAD</span></span>|
|<span data-ttu-id="85a3b-121">Ative</span><span class="sxs-lookup"><span data-stu-id="85a3b-121">retire</span></span>|<span data-ttu-id="85a3b-122">3D</span><span class="sxs-lookup"><span data-stu-id="85a3b-122">3</span></span>|<span data-ttu-id="85a3b-123">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="85a3b-123">Retire the device</span></span>|
|<span data-ttu-id="85a3b-124">revelar</span><span class="sxs-lookup"><span data-stu-id="85a3b-124">wipe</span></span>|<span data-ttu-id="85a3b-125">4 </span><span class="sxs-lookup"><span data-stu-id="85a3b-125">4</span></span>|<span data-ttu-id="85a3b-126">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="85a3b-126">Wipe the device</span></span>|
|<span data-ttu-id="85a3b-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="85a3b-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="85a3b-128">5 </span><span class="sxs-lookup"><span data-stu-id="85a3b-128">5</span></span>|<span data-ttu-id="85a3b-129">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="85a3b-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="85a3b-130">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="85a3b-130">pushNotification</span></span>|<span data-ttu-id="85a3b-131">9 </span><span class="sxs-lookup"><span data-stu-id="85a3b-131">9</span></span>|<span data-ttu-id="85a3b-132">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="85a3b-132">Send push notification to device</span></span>|
|<span data-ttu-id="85a3b-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="85a3b-133">remoteLock</span></span>|<span data-ttu-id="85a3b-134">10 </span><span class="sxs-lookup"><span data-stu-id="85a3b-134">10</span></span>|<span data-ttu-id="85a3b-135">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="85a3b-135">Remotely lock the device</span></span>|






