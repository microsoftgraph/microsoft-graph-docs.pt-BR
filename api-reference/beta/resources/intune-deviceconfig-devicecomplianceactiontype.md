---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 33b18120e5ae0d928fbd7a7a42e87bf7f71d10ec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735845"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="bdd19-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="bdd19-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="bdd19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdd19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdd19-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bdd19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdd19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bdd19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdd19-107">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="bdd19-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="bdd19-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bdd19-108">Members</span></span>
|<span data-ttu-id="bdd19-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bdd19-109">Member</span></span>|<span data-ttu-id="bdd19-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bdd19-110">Value</span></span>|<span data-ttu-id="bdd19-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdd19-112">NoAction</span><span class="sxs-lookup"><span data-stu-id="bdd19-112">noAction</span></span>|<span data-ttu-id="bdd19-113">,0</span><span class="sxs-lookup"><span data-stu-id="bdd19-113">0</span></span>|<span data-ttu-id="bdd19-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="bdd19-114">No Action</span></span>|
|<span data-ttu-id="bdd19-115">Notifica</span><span class="sxs-lookup"><span data-stu-id="bdd19-115">notification</span></span>|<span data-ttu-id="bdd19-116">1</span><span class="sxs-lookup"><span data-stu-id="bdd19-116">1</span></span>|<span data-ttu-id="bdd19-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="bdd19-117">Send Notification</span></span>|
|<span data-ttu-id="bdd19-118">Larga</span><span class="sxs-lookup"><span data-stu-id="bdd19-118">block</span></span>|<span data-ttu-id="bdd19-119">duas</span><span class="sxs-lookup"><span data-stu-id="bdd19-119">2</span></span>|<span data-ttu-id="bdd19-120">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="bdd19-120">Block the device in AAD</span></span>|
|<span data-ttu-id="bdd19-121">Ative</span><span class="sxs-lookup"><span data-stu-id="bdd19-121">retire</span></span>|<span data-ttu-id="bdd19-122">3D</span><span class="sxs-lookup"><span data-stu-id="bdd19-122">3</span></span>|<span data-ttu-id="bdd19-123">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="bdd19-123">Retire the device</span></span>|
|<span data-ttu-id="bdd19-124">revelar</span><span class="sxs-lookup"><span data-stu-id="bdd19-124">wipe</span></span>|<span data-ttu-id="bdd19-125">4 </span><span class="sxs-lookup"><span data-stu-id="bdd19-125">4</span></span>|<span data-ttu-id="bdd19-126">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="bdd19-126">Wipe the device</span></span>|
|<span data-ttu-id="bdd19-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="bdd19-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="bdd19-128">5 </span><span class="sxs-lookup"><span data-stu-id="bdd19-128">5</span></span>|<span data-ttu-id="bdd19-129">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bdd19-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="bdd19-130">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="bdd19-130">pushNotification</span></span>|<span data-ttu-id="bdd19-131">9 </span><span class="sxs-lookup"><span data-stu-id="bdd19-131">9</span></span>|<span data-ttu-id="bdd19-132">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="bdd19-132">Send push notification to device</span></span>|
|<span data-ttu-id="bdd19-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="bdd19-133">remoteLock</span></span>|<span data-ttu-id="bdd19-134">10 </span><span class="sxs-lookup"><span data-stu-id="bdd19-134">10</span></span>|<span data-ttu-id="bdd19-135">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="bdd19-135">Remotely lock the device</span></span>|





