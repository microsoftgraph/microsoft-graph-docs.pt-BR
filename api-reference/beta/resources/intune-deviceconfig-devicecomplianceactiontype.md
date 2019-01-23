---
title: tipo de enum deviceComplianceActionType
description: Enumeração de tipo de ação de agendadas
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425740"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="ed0a7-103">tipo de enum deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ed0a7-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="ed0a7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ed0a7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed0a7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ed0a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed0a7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ed0a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed0a7-107">Enumeração de tipo de ação de agendadas</span><span class="sxs-lookup"><span data-stu-id="ed0a7-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="ed0a7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ed0a7-108">Members</span></span>
|<span data-ttu-id="ed0a7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ed0a7-109">Member</span></span>|<span data-ttu-id="ed0a7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ed0a7-110">Value</span></span>|<span data-ttu-id="ed0a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed0a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed0a7-112">noAction</span><span class="sxs-lookup"><span data-stu-id="ed0a7-112">noAction</span></span>|<span data-ttu-id="ed0a7-113">0</span><span class="sxs-lookup"><span data-stu-id="ed0a7-113">0</span></span>|<span data-ttu-id="ed0a7-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="ed0a7-114">No Action</span></span>|
|<span data-ttu-id="ed0a7-115">notificação</span><span class="sxs-lookup"><span data-stu-id="ed0a7-115">notification</span></span>|<span data-ttu-id="ed0a7-116">1</span><span class="sxs-lookup"><span data-stu-id="ed0a7-116">1</span></span>|<span data-ttu-id="ed0a7-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="ed0a7-117">Send Notification</span></span>|
|<span data-ttu-id="ed0a7-118">bloquear</span><span class="sxs-lookup"><span data-stu-id="ed0a7-118">block</span></span>|<span data-ttu-id="ed0a7-119">2</span><span class="sxs-lookup"><span data-stu-id="ed0a7-119">2</span></span>|<span data-ttu-id="ed0a7-120">Bloquear o dispositivo em AAD</span><span class="sxs-lookup"><span data-stu-id="ed0a7-120">Block the device in AAD</span></span>|
|<span data-ttu-id="ed0a7-121">retirar</span><span class="sxs-lookup"><span data-stu-id="ed0a7-121">retire</span></span>|<span data-ttu-id="ed0a7-122">3</span><span class="sxs-lookup"><span data-stu-id="ed0a7-122">3</span></span>|<span data-ttu-id="ed0a7-123">Desative o dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed0a7-123">Retire the device</span></span>|
|<span data-ttu-id="ed0a7-124">apagar</span><span class="sxs-lookup"><span data-stu-id="ed0a7-124">wipe</span></span>|<span data-ttu-id="ed0a7-125">4</span><span class="sxs-lookup"><span data-stu-id="ed0a7-125">4</span></span>|<span data-ttu-id="ed0a7-126">Apagar dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed0a7-126">Wipe the device</span></span>|
|<span data-ttu-id="ed0a7-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="ed0a7-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="ed0a7-128">5</span><span class="sxs-lookup"><span data-stu-id="ed0a7-128">5</span></span>|<span data-ttu-id="ed0a7-129">Remover o recurso perfis de acesso do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed0a7-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="ed0a7-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="ed0a7-130">pushNotification</span></span>|<span data-ttu-id="ed0a7-131">9</span><span class="sxs-lookup"><span data-stu-id="ed0a7-131">9</span></span>|<span data-ttu-id="ed0a7-132">Enviar notificação por push para dispositivos</span><span class="sxs-lookup"><span data-stu-id="ed0a7-132">Send push notification to device</span></span>|
|<span data-ttu-id="ed0a7-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="ed0a7-133">remoteLock</span></span>|<span data-ttu-id="ed0a7-134">10</span><span class="sxs-lookup"><span data-stu-id="ed0a7-134">10</span></span>|<span data-ttu-id="ed0a7-135">Bloquear remotamente o dispositivo</span><span class="sxs-lookup"><span data-stu-id="ed0a7-135">Remotely lock the device</span></span>|




