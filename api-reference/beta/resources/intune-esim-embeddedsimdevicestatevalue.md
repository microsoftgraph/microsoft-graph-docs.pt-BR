---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb2ab50e9c91f801cc38723a58bed2867c71b347
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528204"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="4e08a-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="4e08a-103">embeddedSIMDeviceStateValue enum type</span></span>

<span data-ttu-id="4e08a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4e08a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e08a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e08a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e08a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e08a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e08a-107">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="4e08a-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="4e08a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4e08a-108">Members</span></span>
|<span data-ttu-id="4e08a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4e08a-109">Member</span></span>|<span data-ttu-id="4e08a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4e08a-110">Value</span></span>|<span data-ttu-id="4e08a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e08a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e08a-112">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="4e08a-112">notEvaluated</span></span>|<span data-ttu-id="4e08a-113">,0</span><span class="sxs-lookup"><span data-stu-id="4e08a-113">0</span></span>|<span data-ttu-id="4e08a-114">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e08a-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="4e08a-115">falhou</span><span class="sxs-lookup"><span data-stu-id="4e08a-115">failed</span></span>|<span data-ttu-id="4e08a-116">1 </span><span class="sxs-lookup"><span data-stu-id="4e08a-116">1</span></span>|<span data-ttu-id="4e08a-117">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e08a-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="4e08a-118">instalado</span><span class="sxs-lookup"><span data-stu-id="4e08a-118">installing</span></span>|<span data-ttu-id="4e08a-119">2 </span><span class="sxs-lookup"><span data-stu-id="4e08a-119">2</span></span>|<span data-ttu-id="4e08a-120">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="4e08a-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="4e08a-121">instalação</span><span class="sxs-lookup"><span data-stu-id="4e08a-121">installed</span></span>|<span data-ttu-id="4e08a-122">3 </span><span class="sxs-lookup"><span data-stu-id="4e08a-122">3</span></span>|<span data-ttu-id="4e08a-123">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="4e08a-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="4e08a-124">deleta</span><span class="sxs-lookup"><span data-stu-id="4e08a-124">deleting</span></span>|<span data-ttu-id="4e08a-125">4 </span><span class="sxs-lookup"><span data-stu-id="4e08a-125">4</span></span>|<span data-ttu-id="4e08a-126">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e08a-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="4e08a-127">erro</span><span class="sxs-lookup"><span data-stu-id="4e08a-127">error</span></span>|<span data-ttu-id="4e08a-128">5 </span><span class="sxs-lookup"><span data-stu-id="4e08a-128">5</span></span>|<span data-ttu-id="4e08a-129">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="4e08a-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="4e08a-130">deleted</span><span class="sxs-lookup"><span data-stu-id="4e08a-130">deleted</span></span>|<span data-ttu-id="4e08a-131">6 </span><span class="sxs-lookup"><span data-stu-id="4e08a-131">6</span></span>|<span data-ttu-id="4e08a-132">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e08a-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="4e08a-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="4e08a-133">removedByUser</span></span>|<span data-ttu-id="4e08a-134">7 </span><span class="sxs-lookup"><span data-stu-id="4e08a-134">7</span></span>|<span data-ttu-id="4e08a-135">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="4e08a-135">Designates that the profile is removed from the device by the user</span></span>|



