---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bff5247237cc0d6daf45515c5bdbaaa3e675017a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526718"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="e46d1-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="e46d1-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="e46d1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e46d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e46d1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e46d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e46d1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e46d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e46d1-107">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="e46d1-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="e46d1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e46d1-108">Members</span></span>
|<span data-ttu-id="e46d1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e46d1-109">Member</span></span>|<span data-ttu-id="e46d1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e46d1-110">Value</span></span>|<span data-ttu-id="e46d1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e46d1-112">NoAction</span><span class="sxs-lookup"><span data-stu-id="e46d1-112">noAction</span></span>|<span data-ttu-id="e46d1-113">,0</span><span class="sxs-lookup"><span data-stu-id="e46d1-113">0</span></span>|<span data-ttu-id="e46d1-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="e46d1-114">No Action</span></span>|
|<span data-ttu-id="e46d1-115">Notifica</span><span class="sxs-lookup"><span data-stu-id="e46d1-115">notification</span></span>|<span data-ttu-id="e46d1-116">1 </span><span class="sxs-lookup"><span data-stu-id="e46d1-116">1</span></span>|<span data-ttu-id="e46d1-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="e46d1-117">Send Notification</span></span>|
|<span data-ttu-id="e46d1-118">Larga</span><span class="sxs-lookup"><span data-stu-id="e46d1-118">block</span></span>|<span data-ttu-id="e46d1-119">2 </span><span class="sxs-lookup"><span data-stu-id="e46d1-119">2</span></span>|<span data-ttu-id="e46d1-120">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="e46d1-120">Block the device in AAD</span></span>|
|<span data-ttu-id="e46d1-121">Ative</span><span class="sxs-lookup"><span data-stu-id="e46d1-121">retire</span></span>|<span data-ttu-id="e46d1-122">3 </span><span class="sxs-lookup"><span data-stu-id="e46d1-122">3</span></span>|<span data-ttu-id="e46d1-123">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e46d1-123">Retire the device</span></span>|
|<span data-ttu-id="e46d1-124">revelar</span><span class="sxs-lookup"><span data-stu-id="e46d1-124">wipe</span></span>|<span data-ttu-id="e46d1-125">4 </span><span class="sxs-lookup"><span data-stu-id="e46d1-125">4</span></span>|<span data-ttu-id="e46d1-126">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e46d1-126">Wipe the device</span></span>|
|<span data-ttu-id="e46d1-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="e46d1-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="e46d1-128">5 </span><span class="sxs-lookup"><span data-stu-id="e46d1-128">5</span></span>|<span data-ttu-id="e46d1-129">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e46d1-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="e46d1-130">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="e46d1-130">pushNotification</span></span>|<span data-ttu-id="e46d1-131">9 </span><span class="sxs-lookup"><span data-stu-id="e46d1-131">9</span></span>|<span data-ttu-id="e46d1-132">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="e46d1-132">Send push notification to device</span></span>|
|<span data-ttu-id="e46d1-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="e46d1-133">remoteLock</span></span>|<span data-ttu-id="e46d1-134">10 </span><span class="sxs-lookup"><span data-stu-id="e46d1-134">10</span></span>|<span data-ttu-id="e46d1-135">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="e46d1-135">Remotely lock the device</span></span>|



