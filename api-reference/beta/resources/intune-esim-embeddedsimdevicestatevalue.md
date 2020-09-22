---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4529f189940470447a0f3aca151bc7b285d5ab2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031435"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="b23ba-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="b23ba-103">embeddedSIMDeviceStateValue enum type</span></span>

<span data-ttu-id="b23ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b23ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b23ba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b23ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b23ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b23ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b23ba-107">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="b23ba-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="b23ba-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b23ba-108">Members</span></span>
|<span data-ttu-id="b23ba-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b23ba-109">Member</span></span>|<span data-ttu-id="b23ba-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b23ba-110">Value</span></span>|<span data-ttu-id="b23ba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b23ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23ba-112">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="b23ba-112">notEvaluated</span></span>|<span data-ttu-id="b23ba-113">,0</span><span class="sxs-lookup"><span data-stu-id="b23ba-113">0</span></span>|<span data-ttu-id="b23ba-114">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b23ba-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="b23ba-115">falhou</span><span class="sxs-lookup"><span data-stu-id="b23ba-115">failed</span></span>|<span data-ttu-id="b23ba-116">1 </span><span class="sxs-lookup"><span data-stu-id="b23ba-116">1</span></span>|<span data-ttu-id="b23ba-117">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b23ba-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="b23ba-118">instalado</span><span class="sxs-lookup"><span data-stu-id="b23ba-118">installing</span></span>|<span data-ttu-id="b23ba-119">2 </span><span class="sxs-lookup"><span data-stu-id="b23ba-119">2</span></span>|<span data-ttu-id="b23ba-120">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="b23ba-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="b23ba-121">instalação</span><span class="sxs-lookup"><span data-stu-id="b23ba-121">installed</span></span>|<span data-ttu-id="b23ba-122">3 </span><span class="sxs-lookup"><span data-stu-id="b23ba-122">3</span></span>|<span data-ttu-id="b23ba-123">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="b23ba-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="b23ba-124">deleta</span><span class="sxs-lookup"><span data-stu-id="b23ba-124">deleting</span></span>|<span data-ttu-id="b23ba-125">4 </span><span class="sxs-lookup"><span data-stu-id="b23ba-125">4</span></span>|<span data-ttu-id="b23ba-126">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b23ba-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="b23ba-127">erro</span><span class="sxs-lookup"><span data-stu-id="b23ba-127">error</span></span>|<span data-ttu-id="b23ba-128">5 </span><span class="sxs-lookup"><span data-stu-id="b23ba-128">5</span></span>|<span data-ttu-id="b23ba-129">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="b23ba-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="b23ba-130">deleted</span><span class="sxs-lookup"><span data-stu-id="b23ba-130">deleted</span></span>|<span data-ttu-id="b23ba-131">6 </span><span class="sxs-lookup"><span data-stu-id="b23ba-131">6</span></span>|<span data-ttu-id="b23ba-132">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b23ba-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="b23ba-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="b23ba-133">removedByUser</span></span>|<span data-ttu-id="b23ba-134">7 </span><span class="sxs-lookup"><span data-stu-id="b23ba-134">7</span></span>|<span data-ttu-id="b23ba-135">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="b23ba-135">Designates that the profile is removed from the device by the user</span></span>|






