---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c36d6739e13027f2a4136899e0e60a4dbff8d990
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998776"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="1ce4e-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="1ce4e-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="1ce4e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ce4e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce4e-106">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="1ce4e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1ce4e-107">Members</span></span>
|<span data-ttu-id="1ce4e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1ce4e-108">Member</span></span>|<span data-ttu-id="1ce4e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1ce4e-109">Value</span></span>|<span data-ttu-id="1ce4e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ce4e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce4e-111">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="1ce4e-111">notEvaluated</span></span>|<span data-ttu-id="1ce4e-112">,0</span><span class="sxs-lookup"><span data-stu-id="1ce4e-112">0</span></span>|<span data-ttu-id="1ce4e-113">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="1ce4e-114">falhou</span><span class="sxs-lookup"><span data-stu-id="1ce4e-114">failed</span></span>|<span data-ttu-id="1ce4e-115">1</span><span class="sxs-lookup"><span data-stu-id="1ce4e-115">1</span></span>|<span data-ttu-id="1ce4e-116">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="1ce4e-117">instalado</span><span class="sxs-lookup"><span data-stu-id="1ce4e-117">installing</span></span>|<span data-ttu-id="1ce4e-118">duas</span><span class="sxs-lookup"><span data-stu-id="1ce4e-118">2</span></span>|<span data-ttu-id="1ce4e-119">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="1ce4e-120">instalação</span><span class="sxs-lookup"><span data-stu-id="1ce4e-120">installed</span></span>|<span data-ttu-id="1ce4e-121">3D</span><span class="sxs-lookup"><span data-stu-id="1ce4e-121">3</span></span>|<span data-ttu-id="1ce4e-122">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="1ce4e-123">deleta</span><span class="sxs-lookup"><span data-stu-id="1ce4e-123">deleting</span></span>|<span data-ttu-id="1ce4e-124">quatro</span><span class="sxs-lookup"><span data-stu-id="1ce4e-124">4</span></span>|<span data-ttu-id="1ce4e-125">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="1ce4e-126">erro</span><span class="sxs-lookup"><span data-stu-id="1ce4e-126">error</span></span>|<span data-ttu-id="1ce4e-127">0,5</span><span class="sxs-lookup"><span data-stu-id="1ce4e-127">5</span></span>|<span data-ttu-id="1ce4e-128">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="1ce4e-129">deleted</span><span class="sxs-lookup"><span data-stu-id="1ce4e-129">deleted</span></span>|<span data-ttu-id="1ce4e-130">6</span><span class="sxs-lookup"><span data-stu-id="1ce4e-130">6</span></span>|<span data-ttu-id="1ce4e-131">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ce4e-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="1ce4e-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="1ce4e-132">removedByUser</span></span>|<span data-ttu-id="1ce4e-133">178</span><span class="sxs-lookup"><span data-stu-id="1ce4e-133">7</span></span>|<span data-ttu-id="1ce4e-134">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="1ce4e-134">Designates that the profile is removed from the device by the user</span></span>|





