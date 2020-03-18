---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4ebf4df22787d19e5718ebd2099cd81af3925271
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793356"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="1020b-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="1020b-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="1020b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1020b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1020b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1020b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1020b-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="1020b-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="1020b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1020b-107">Members</span></span>
|<span data-ttu-id="1020b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1020b-108">Member</span></span>|<span data-ttu-id="1020b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1020b-109">Value</span></span>|<span data-ttu-id="1020b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1020b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1020b-111">NoAction</span><span class="sxs-lookup"><span data-stu-id="1020b-111">noAction</span></span>|<span data-ttu-id="1020b-112">,0</span><span class="sxs-lookup"><span data-stu-id="1020b-112">0</span></span>|<span data-ttu-id="1020b-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="1020b-113">No Action</span></span>|
|<span data-ttu-id="1020b-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="1020b-114">notification</span></span>|<span data-ttu-id="1020b-115">1</span><span class="sxs-lookup"><span data-stu-id="1020b-115">1</span></span>|<span data-ttu-id="1020b-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="1020b-116">Send Notification</span></span>|
|<span data-ttu-id="1020b-117">Larga</span><span class="sxs-lookup"><span data-stu-id="1020b-117">block</span></span>|<span data-ttu-id="1020b-118">duas</span><span class="sxs-lookup"><span data-stu-id="1020b-118">2</span></span>|<span data-ttu-id="1020b-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="1020b-119">Block the device in AAD</span></span>|
|<span data-ttu-id="1020b-120">Ative</span><span class="sxs-lookup"><span data-stu-id="1020b-120">retire</span></span>|<span data-ttu-id="1020b-121">3D</span><span class="sxs-lookup"><span data-stu-id="1020b-121">3</span></span>|<span data-ttu-id="1020b-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1020b-122">Retire the device</span></span>|
|<span data-ttu-id="1020b-123">revelar</span><span class="sxs-lookup"><span data-stu-id="1020b-123">wipe</span></span>|<span data-ttu-id="1020b-124">4 </span><span class="sxs-lookup"><span data-stu-id="1020b-124">4</span></span>|<span data-ttu-id="1020b-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1020b-125">Wipe the device</span></span>|
|<span data-ttu-id="1020b-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="1020b-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="1020b-127">5 </span><span class="sxs-lookup"><span data-stu-id="1020b-127">5</span></span>|<span data-ttu-id="1020b-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1020b-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="1020b-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="1020b-129">pushNotification</span></span>|<span data-ttu-id="1020b-130">9 </span><span class="sxs-lookup"><span data-stu-id="1020b-130">9</span></span>|<span data-ttu-id="1020b-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="1020b-131">Send push notification to device</span></span>|
|<span data-ttu-id="1020b-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="1020b-132">remoteLock</span></span>|<span data-ttu-id="1020b-133">10 </span><span class="sxs-lookup"><span data-stu-id="1020b-133">10</span></span>|<span data-ttu-id="1020b-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="1020b-134">Remotely lock the device</span></span>|



