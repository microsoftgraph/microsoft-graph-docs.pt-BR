---
title: tipo de enumeração Enumeraçãodevicecomplianceactiontype
description: Enumeração de tipo de ação agendada
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566028"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="81307-103">tipo de enumeração Enumeraçãodevicecomplianceactiontype</span><span class="sxs-lookup"><span data-stu-id="81307-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="81307-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81307-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81307-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81307-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81307-106">Enumeração de tipo de ação agendada</span><span class="sxs-lookup"><span data-stu-id="81307-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="81307-107">Membros</span><span class="sxs-lookup"><span data-stu-id="81307-107">Members</span></span>
|<span data-ttu-id="81307-108">Membro</span><span class="sxs-lookup"><span data-stu-id="81307-108">Member</span></span>|<span data-ttu-id="81307-109">Valor</span><span class="sxs-lookup"><span data-stu-id="81307-109">Value</span></span>|<span data-ttu-id="81307-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81307-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81307-111">noAction</span><span class="sxs-lookup"><span data-stu-id="81307-111">noAction</span></span>|<span data-ttu-id="81307-112">,0</span><span class="sxs-lookup"><span data-stu-id="81307-112">0</span></span>|<span data-ttu-id="81307-113">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="81307-113">No Action</span></span>|
|<span data-ttu-id="81307-114">Notifica</span><span class="sxs-lookup"><span data-stu-id="81307-114">notification</span></span>|<span data-ttu-id="81307-115">1 </span><span class="sxs-lookup"><span data-stu-id="81307-115">1</span></span>|<span data-ttu-id="81307-116">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="81307-116">Send Notification</span></span>|
|<span data-ttu-id="81307-117">Larga</span><span class="sxs-lookup"><span data-stu-id="81307-117">block</span></span>|<span data-ttu-id="81307-118">2 </span><span class="sxs-lookup"><span data-stu-id="81307-118">2</span></span>|<span data-ttu-id="81307-119">Bloquear o dispositivo no AAD</span><span class="sxs-lookup"><span data-stu-id="81307-119">Block the device in AAD</span></span>|
|<span data-ttu-id="81307-120">Ative</span><span class="sxs-lookup"><span data-stu-id="81307-120">retire</span></span>|<span data-ttu-id="81307-121">3 </span><span class="sxs-lookup"><span data-stu-id="81307-121">3</span></span>|<span data-ttu-id="81307-122">Desativar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="81307-122">Retire the device</span></span>|
|<span data-ttu-id="81307-123">revelar</span><span class="sxs-lookup"><span data-stu-id="81307-123">wipe</span></span>|<span data-ttu-id="81307-124">4 </span><span class="sxs-lookup"><span data-stu-id="81307-124">4</span></span>|<span data-ttu-id="81307-125">Apagar o dispositivo</span><span class="sxs-lookup"><span data-stu-id="81307-125">Wipe the device</span></span>|
|<span data-ttu-id="81307-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="81307-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="81307-127">5 </span><span class="sxs-lookup"><span data-stu-id="81307-127">5</span></span>|<span data-ttu-id="81307-128">Remover perfis de acesso a recursos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="81307-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="81307-129">Membropushnotification</span><span class="sxs-lookup"><span data-stu-id="81307-129">pushNotification</span></span>|<span data-ttu-id="81307-130">9 </span><span class="sxs-lookup"><span data-stu-id="81307-130">9</span></span>|<span data-ttu-id="81307-131">Enviar notificação por push ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="81307-131">Send push notification to device</span></span>|
|<span data-ttu-id="81307-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="81307-132">remoteLock</span></span>|<span data-ttu-id="81307-133">10 </span><span class="sxs-lookup"><span data-stu-id="81307-133">10</span></span>|<span data-ttu-id="81307-134">Bloquear o dispositivo remotamente</span><span class="sxs-lookup"><span data-stu-id="81307-134">Remotely lock the device</span></span>|





