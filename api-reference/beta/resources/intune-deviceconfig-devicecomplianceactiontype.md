---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9409ddebd69d8b046c522de1c3e58baabc15a2ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970616"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="d511a-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="d511a-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="d511a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d511a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d511a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d511a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d511a-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="d511a-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="d511a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d511a-107">Members</span></span>
|<span data-ttu-id="d511a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d511a-108">Member</span></span>|<span data-ttu-id="d511a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d511a-109">Value</span></span>|<span data-ttu-id="d511a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d511a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d511a-111">NoAction</span><span class="sxs-lookup"><span data-stu-id="d511a-111">noAction</span></span>|<span data-ttu-id="d511a-112">,0</span><span class="sxs-lookup"><span data-stu-id="d511a-112">0</span></span>|<span data-ttu-id="d511a-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="d511a-113">No Action</span></span>|
|<span data-ttu-id="d511a-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="d511a-114">notification</span></span>|<span data-ttu-id="d511a-115">1</span><span class="sxs-lookup"><span data-stu-id="d511a-115">1</span></span>|<span data-ttu-id="d511a-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="d511a-116">Send Notification</span></span>|
|<span data-ttu-id="d511a-117">Larga</span><span class="sxs-lookup"><span data-stu-id="d511a-117">block</span></span>|<span data-ttu-id="d511a-118">duas</span><span class="sxs-lookup"><span data-stu-id="d511a-118">2</span></span>|<span data-ttu-id="d511a-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="d511a-119">Block the device in AAD</span></span>|
|<span data-ttu-id="d511a-120">Ative</span><span class="sxs-lookup"><span data-stu-id="d511a-120">retire</span></span>|<span data-ttu-id="d511a-121">3D</span><span class="sxs-lookup"><span data-stu-id="d511a-121">3</span></span>|<span data-ttu-id="d511a-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d511a-122">Retire the device</span></span>|
|<span data-ttu-id="d511a-123">revelar</span><span class="sxs-lookup"><span data-stu-id="d511a-123">wipe</span></span>|<span data-ttu-id="d511a-124">quatro</span><span class="sxs-lookup"><span data-stu-id="d511a-124">4</span></span>|<span data-ttu-id="d511a-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d511a-125">Wipe the device</span></span>|
|<span data-ttu-id="d511a-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="d511a-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="d511a-127">0,5</span><span class="sxs-lookup"><span data-stu-id="d511a-127">5</span></span>|<span data-ttu-id="d511a-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d511a-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="d511a-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="d511a-129">pushNotification</span></span>|<span data-ttu-id="d511a-130">9 </span><span class="sxs-lookup"><span data-stu-id="d511a-130">9</span></span>|<span data-ttu-id="d511a-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="d511a-131">Send push notification to device</span></span>|
|<span data-ttu-id="d511a-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="d511a-132">remoteLock</span></span>|<span data-ttu-id="d511a-133">10 </span><span class="sxs-lookup"><span data-stu-id="d511a-133">10</span></span>|<span data-ttu-id="d511a-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="d511a-134">Remotely lock the device</span></span>|





