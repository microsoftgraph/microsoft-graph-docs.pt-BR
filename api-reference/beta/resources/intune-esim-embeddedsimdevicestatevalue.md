---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bdc3250605de7db7a3778d64b5e743a415de4c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145420"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="fb48a-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="fb48a-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="fb48a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb48a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb48a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb48a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb48a-106">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="fb48a-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="fb48a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fb48a-107">Members</span></span>
|<span data-ttu-id="fb48a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fb48a-108">Member</span></span>|<span data-ttu-id="fb48a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fb48a-109">Value</span></span>|<span data-ttu-id="fb48a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb48a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb48a-111">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="fb48a-111">notEvaluated</span></span>|<span data-ttu-id="fb48a-112">,0</span><span class="sxs-lookup"><span data-stu-id="fb48a-112">0</span></span>|<span data-ttu-id="fb48a-113">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb48a-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="fb48a-114">falhou</span><span class="sxs-lookup"><span data-stu-id="fb48a-114">failed</span></span>|<span data-ttu-id="fb48a-115">1</span><span class="sxs-lookup"><span data-stu-id="fb48a-115">1</span></span>|<span data-ttu-id="fb48a-116">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb48a-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="fb48a-117">instalado</span><span class="sxs-lookup"><span data-stu-id="fb48a-117">installing</span></span>|<span data-ttu-id="fb48a-118">duas</span><span class="sxs-lookup"><span data-stu-id="fb48a-118">2</span></span>|<span data-ttu-id="fb48a-119">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="fb48a-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="fb48a-120">instalação</span><span class="sxs-lookup"><span data-stu-id="fb48a-120">installed</span></span>|<span data-ttu-id="fb48a-121">3D</span><span class="sxs-lookup"><span data-stu-id="fb48a-121">3</span></span>|<span data-ttu-id="fb48a-122">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="fb48a-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="fb48a-123">deleta</span><span class="sxs-lookup"><span data-stu-id="fb48a-123">deleting</span></span>|<span data-ttu-id="fb48a-124">quatro</span><span class="sxs-lookup"><span data-stu-id="fb48a-124">4</span></span>|<span data-ttu-id="fb48a-125">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb48a-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="fb48a-126">erro</span><span class="sxs-lookup"><span data-stu-id="fb48a-126">error</span></span>|<span data-ttu-id="fb48a-127">0,5</span><span class="sxs-lookup"><span data-stu-id="fb48a-127">5</span></span>|<span data-ttu-id="fb48a-128">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="fb48a-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="fb48a-129">deleted</span><span class="sxs-lookup"><span data-stu-id="fb48a-129">deleted</span></span>|<span data-ttu-id="fb48a-130">6</span><span class="sxs-lookup"><span data-stu-id="fb48a-130">6</span></span>|<span data-ttu-id="fb48a-131">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb48a-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="fb48a-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="fb48a-132">removedByUser</span></span>|<span data-ttu-id="fb48a-133">178</span><span class="sxs-lookup"><span data-stu-id="fb48a-133">7</span></span>|<span data-ttu-id="fb48a-134">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="fb48a-134">Designates that the profile is removed from the device by the user</span></span>|




