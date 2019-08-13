---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a4369a891af8ebdda818a0e7b62d4c8d827d029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326713"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="bc1cf-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="bc1cf-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="bc1cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc1cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc1cf-106">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="bc1cf-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bc1cf-107">Members</span></span>
|<span data-ttu-id="bc1cf-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bc1cf-108">Member</span></span>|<span data-ttu-id="bc1cf-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bc1cf-109">Value</span></span>|<span data-ttu-id="bc1cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc1cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc1cf-111">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="bc1cf-111">notEvaluated</span></span>|<span data-ttu-id="bc1cf-112">,0</span><span class="sxs-lookup"><span data-stu-id="bc1cf-112">0</span></span>|<span data-ttu-id="bc1cf-113">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="bc1cf-114">falhou</span><span class="sxs-lookup"><span data-stu-id="bc1cf-114">failed</span></span>|<span data-ttu-id="bc1cf-115">1</span><span class="sxs-lookup"><span data-stu-id="bc1cf-115">1</span></span>|<span data-ttu-id="bc1cf-116">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="bc1cf-117">instalado</span><span class="sxs-lookup"><span data-stu-id="bc1cf-117">installing</span></span>|<span data-ttu-id="bc1cf-118">duas</span><span class="sxs-lookup"><span data-stu-id="bc1cf-118">2</span></span>|<span data-ttu-id="bc1cf-119">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="bc1cf-120">instalação</span><span class="sxs-lookup"><span data-stu-id="bc1cf-120">installed</span></span>|<span data-ttu-id="bc1cf-121">3D</span><span class="sxs-lookup"><span data-stu-id="bc1cf-121">3</span></span>|<span data-ttu-id="bc1cf-122">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="bc1cf-123">deleta</span><span class="sxs-lookup"><span data-stu-id="bc1cf-123">deleting</span></span>|<span data-ttu-id="bc1cf-124">quatro</span><span class="sxs-lookup"><span data-stu-id="bc1cf-124">4</span></span>|<span data-ttu-id="bc1cf-125">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="bc1cf-126">erro</span><span class="sxs-lookup"><span data-stu-id="bc1cf-126">error</span></span>|<span data-ttu-id="bc1cf-127">0,5</span><span class="sxs-lookup"><span data-stu-id="bc1cf-127">5</span></span>|<span data-ttu-id="bc1cf-128">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="bc1cf-129">deleted</span><span class="sxs-lookup"><span data-stu-id="bc1cf-129">deleted</span></span>|<span data-ttu-id="bc1cf-130">6</span><span class="sxs-lookup"><span data-stu-id="bc1cf-130">6</span></span>|<span data-ttu-id="bc1cf-131">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc1cf-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="bc1cf-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="bc1cf-132">removedByUser</span></span>|<span data-ttu-id="bc1cf-133">178</span><span class="sxs-lookup"><span data-stu-id="bc1cf-133">7</span></span>|<span data-ttu-id="bc1cf-134">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="bc1cf-134">Designates that the profile is removed from the device by the user</span></span>|



