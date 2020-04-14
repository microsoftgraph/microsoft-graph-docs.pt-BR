---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0a5a3b4ab73bc0d97b5b47619cdcabb401400f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437389"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="86854-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="86854-103">deviceComplianceActionType enum type</span></span>

<span data-ttu-id="86854-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86854-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86854-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86854-107">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="86854-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="86854-108">Membros</span><span class="sxs-lookup"><span data-stu-id="86854-108">Members</span></span>
|<span data-ttu-id="86854-109">Membro</span><span class="sxs-lookup"><span data-stu-id="86854-109">Member</span></span>|<span data-ttu-id="86854-110">Valor</span><span class="sxs-lookup"><span data-stu-id="86854-110">Value</span></span>|<span data-ttu-id="86854-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86854-112">NoAction</span><span class="sxs-lookup"><span data-stu-id="86854-112">noAction</span></span>|<span data-ttu-id="86854-113">,0</span><span class="sxs-lookup"><span data-stu-id="86854-113">0</span></span>|<span data-ttu-id="86854-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="86854-114">No Action</span></span>|
|<span data-ttu-id="86854-115">Notifica</span><span class="sxs-lookup"><span data-stu-id="86854-115">notification</span></span>|<span data-ttu-id="86854-116">1</span><span class="sxs-lookup"><span data-stu-id="86854-116">1</span></span>|<span data-ttu-id="86854-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="86854-117">Send Notification</span></span>|
|<span data-ttu-id="86854-118">Larga</span><span class="sxs-lookup"><span data-stu-id="86854-118">block</span></span>|<span data-ttu-id="86854-119">duas</span><span class="sxs-lookup"><span data-stu-id="86854-119">2</span></span>|<span data-ttu-id="86854-120">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="86854-120">Block the device in AAD</span></span>|
|<span data-ttu-id="86854-121">Ative</span><span class="sxs-lookup"><span data-stu-id="86854-121">retire</span></span>|<span data-ttu-id="86854-122">3D</span><span class="sxs-lookup"><span data-stu-id="86854-122">3</span></span>|<span data-ttu-id="86854-123">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="86854-123">Retire the device</span></span>|
|<span data-ttu-id="86854-124">revelar</span><span class="sxs-lookup"><span data-stu-id="86854-124">wipe</span></span>|<span data-ttu-id="86854-125">4 </span><span class="sxs-lookup"><span data-stu-id="86854-125">4</span></span>|<span data-ttu-id="86854-126">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="86854-126">Wipe the device</span></span>|
|<span data-ttu-id="86854-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="86854-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="86854-128">5 </span><span class="sxs-lookup"><span data-stu-id="86854-128">5</span></span>|<span data-ttu-id="86854-129">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="86854-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="86854-130">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="86854-130">pushNotification</span></span>|<span data-ttu-id="86854-131">9 </span><span class="sxs-lookup"><span data-stu-id="86854-131">9</span></span>|<span data-ttu-id="86854-132">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="86854-132">Send push notification to device</span></span>|
|<span data-ttu-id="86854-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="86854-133">remoteLock</span></span>|<span data-ttu-id="86854-134">10 </span><span class="sxs-lookup"><span data-stu-id="86854-134">10</span></span>|<span data-ttu-id="86854-135">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="86854-135">Remotely lock the device</span></span>|



