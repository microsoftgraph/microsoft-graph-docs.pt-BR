---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b2af0545dda4461115ed5f11975a6c9371d4010d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283676"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="0672d-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="0672d-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="0672d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0672d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0672d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0672d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0672d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0672d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0672d-107">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="0672d-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="0672d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0672d-108">Members</span></span>
|<span data-ttu-id="0672d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0672d-109">Member</span></span>|<span data-ttu-id="0672d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0672d-110">Value</span></span>|<span data-ttu-id="0672d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0672d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0672d-112">NoAction</span><span class="sxs-lookup"><span data-stu-id="0672d-112">noAction</span></span>|<span data-ttu-id="0672d-113">,0</span><span class="sxs-lookup"><span data-stu-id="0672d-113">0</span></span>|<span data-ttu-id="0672d-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="0672d-114">No Action</span></span>|
|<span data-ttu-id="0672d-115">Notifica</span><span class="sxs-lookup"><span data-stu-id="0672d-115">notification</span></span>|<span data-ttu-id="0672d-116">1</span><span class="sxs-lookup"><span data-stu-id="0672d-116">1</span></span>|<span data-ttu-id="0672d-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="0672d-117">Send Notification</span></span>|
|<span data-ttu-id="0672d-118">Larga</span><span class="sxs-lookup"><span data-stu-id="0672d-118">block</span></span>|<span data-ttu-id="0672d-119">duas</span><span class="sxs-lookup"><span data-stu-id="0672d-119">2</span></span>|<span data-ttu-id="0672d-120">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="0672d-120">Block the device in AAD</span></span>|
|<span data-ttu-id="0672d-121">Ative</span><span class="sxs-lookup"><span data-stu-id="0672d-121">retire</span></span>|<span data-ttu-id="0672d-122">3D</span><span class="sxs-lookup"><span data-stu-id="0672d-122">3</span></span>|<span data-ttu-id="0672d-123">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="0672d-123">Retire the device</span></span>|
|<span data-ttu-id="0672d-124">revelar</span><span class="sxs-lookup"><span data-stu-id="0672d-124">wipe</span></span>|<span data-ttu-id="0672d-125">4 </span><span class="sxs-lookup"><span data-stu-id="0672d-125">4</span></span>|<span data-ttu-id="0672d-126">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="0672d-126">Wipe the device</span></span>|
|<span data-ttu-id="0672d-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="0672d-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="0672d-128">5 </span><span class="sxs-lookup"><span data-stu-id="0672d-128">5</span></span>|<span data-ttu-id="0672d-129">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0672d-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="0672d-130">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="0672d-130">pushNotification</span></span>|<span data-ttu-id="0672d-131">9 </span><span class="sxs-lookup"><span data-stu-id="0672d-131">9</span></span>|<span data-ttu-id="0672d-132">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="0672d-132">Send push notification to device</span></span>|
|<span data-ttu-id="0672d-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="0672d-133">remoteLock</span></span>|<span data-ttu-id="0672d-134">10 </span><span class="sxs-lookup"><span data-stu-id="0672d-134">10</span></span>|<span data-ttu-id="0672d-135">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="0672d-135">Remotely lock the device</span></span>|




