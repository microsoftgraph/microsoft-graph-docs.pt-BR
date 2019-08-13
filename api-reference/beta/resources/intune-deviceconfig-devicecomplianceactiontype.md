---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ab26d2b6cda774f3d2cf3284f92d1901cc4bdf82
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333209"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="16567-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="16567-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="16567-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16567-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16567-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16567-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16567-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="16567-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="16567-107">Membros</span><span class="sxs-lookup"><span data-stu-id="16567-107">Members</span></span>
|<span data-ttu-id="16567-108">Membro</span><span class="sxs-lookup"><span data-stu-id="16567-108">Member</span></span>|<span data-ttu-id="16567-109">Valor</span><span class="sxs-lookup"><span data-stu-id="16567-109">Value</span></span>|<span data-ttu-id="16567-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="16567-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16567-111">NoAction</span><span class="sxs-lookup"><span data-stu-id="16567-111">noAction</span></span>|<span data-ttu-id="16567-112">,0</span><span class="sxs-lookup"><span data-stu-id="16567-112">0</span></span>|<span data-ttu-id="16567-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="16567-113">No Action</span></span>|
|<span data-ttu-id="16567-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="16567-114">notification</span></span>|<span data-ttu-id="16567-115">1</span><span class="sxs-lookup"><span data-stu-id="16567-115">1</span></span>|<span data-ttu-id="16567-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="16567-116">Send Notification</span></span>|
|<span data-ttu-id="16567-117">Larga</span><span class="sxs-lookup"><span data-stu-id="16567-117">block</span></span>|<span data-ttu-id="16567-118">duas</span><span class="sxs-lookup"><span data-stu-id="16567-118">2</span></span>|<span data-ttu-id="16567-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="16567-119">Block the device in AAD</span></span>|
|<span data-ttu-id="16567-120">Ative</span><span class="sxs-lookup"><span data-stu-id="16567-120">retire</span></span>|<span data-ttu-id="16567-121">3D</span><span class="sxs-lookup"><span data-stu-id="16567-121">3</span></span>|<span data-ttu-id="16567-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="16567-122">Retire the device</span></span>|
|<span data-ttu-id="16567-123">revelar</span><span class="sxs-lookup"><span data-stu-id="16567-123">wipe</span></span>|<span data-ttu-id="16567-124">quatro</span><span class="sxs-lookup"><span data-stu-id="16567-124">4</span></span>|<span data-ttu-id="16567-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="16567-125">Wipe the device</span></span>|
|<span data-ttu-id="16567-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="16567-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="16567-127">0,5</span><span class="sxs-lookup"><span data-stu-id="16567-127">5</span></span>|<span data-ttu-id="16567-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="16567-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="16567-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="16567-129">pushNotification</span></span>|<span data-ttu-id="16567-130">9 </span><span class="sxs-lookup"><span data-stu-id="16567-130">9</span></span>|<span data-ttu-id="16567-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="16567-131">Send push notification to device</span></span>|
|<span data-ttu-id="16567-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="16567-132">remoteLock</span></span>|<span data-ttu-id="16567-133">10 </span><span class="sxs-lookup"><span data-stu-id="16567-133">10</span></span>|<span data-ttu-id="16567-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="16567-134">Remotely lock the device</span></span>|



