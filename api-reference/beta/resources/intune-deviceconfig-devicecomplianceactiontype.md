---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d824f579787bf24cc56704a1c8a9df280d969809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173504"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="dda27-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="dda27-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="dda27-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dda27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dda27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dda27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dda27-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="dda27-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="dda27-107">Membros</span><span class="sxs-lookup"><span data-stu-id="dda27-107">Members</span></span>
|<span data-ttu-id="dda27-108">Membro</span><span class="sxs-lookup"><span data-stu-id="dda27-108">Member</span></span>|<span data-ttu-id="dda27-109">Valor</span><span class="sxs-lookup"><span data-stu-id="dda27-109">Value</span></span>|<span data-ttu-id="dda27-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dda27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dda27-111">noAction</span><span class="sxs-lookup"><span data-stu-id="dda27-111">noAction</span></span>|<span data-ttu-id="dda27-112">,0</span><span class="sxs-lookup"><span data-stu-id="dda27-112">0</span></span>|<span data-ttu-id="dda27-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="dda27-113">No Action</span></span>|
|<span data-ttu-id="dda27-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="dda27-114">notification</span></span>|<span data-ttu-id="dda27-115">1</span><span class="sxs-lookup"><span data-stu-id="dda27-115">1</span></span>|<span data-ttu-id="dda27-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="dda27-116">Send Notification</span></span>|
|<span data-ttu-id="dda27-117">Larga</span><span class="sxs-lookup"><span data-stu-id="dda27-117">block</span></span>|<span data-ttu-id="dda27-118">duas</span><span class="sxs-lookup"><span data-stu-id="dda27-118">2</span></span>|<span data-ttu-id="dda27-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="dda27-119">Block the device in AAD</span></span>|
|<span data-ttu-id="dda27-120">Ative</span><span class="sxs-lookup"><span data-stu-id="dda27-120">retire</span></span>|<span data-ttu-id="dda27-121">3D</span><span class="sxs-lookup"><span data-stu-id="dda27-121">3</span></span>|<span data-ttu-id="dda27-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="dda27-122">Retire the device</span></span>|
|<span data-ttu-id="dda27-123">revelar</span><span class="sxs-lookup"><span data-stu-id="dda27-123">wipe</span></span>|<span data-ttu-id="dda27-124">quatro</span><span class="sxs-lookup"><span data-stu-id="dda27-124">4</span></span>|<span data-ttu-id="dda27-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="dda27-125">Wipe the device</span></span>|
|<span data-ttu-id="dda27-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="dda27-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="dda27-127">0,5</span><span class="sxs-lookup"><span data-stu-id="dda27-127">5</span></span>|<span data-ttu-id="dda27-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="dda27-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="dda27-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="dda27-129">pushNotification</span></span>|<span data-ttu-id="dda27-130">241</span><span class="sxs-lookup"><span data-stu-id="dda27-130">9</span></span>|<span data-ttu-id="dda27-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="dda27-131">Send push notification to device</span></span>|
|<span data-ttu-id="dda27-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="dda27-132">remoteLock</span></span>|<span data-ttu-id="dda27-133">254</span><span class="sxs-lookup"><span data-stu-id="dda27-133">10</span></span>|<span data-ttu-id="dda27-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="dda27-134">Remotely lock the device</span></span>|




