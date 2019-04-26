---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a4970e08ff9b305aaf2aad4d82daf994d2010bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568763"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="85eed-103">tipo de enumeração embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="85eed-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="85eed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85eed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85eed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85eed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85eed-106">Descreve os vários Estados de um código de ativação do SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="85eed-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="85eed-107">Membros</span><span class="sxs-lookup"><span data-stu-id="85eed-107">Members</span></span>
|<span data-ttu-id="85eed-108">Membro</span><span class="sxs-lookup"><span data-stu-id="85eed-108">Member</span></span>|<span data-ttu-id="85eed-109">Valor</span><span class="sxs-lookup"><span data-stu-id="85eed-109">Value</span></span>|<span data-ttu-id="85eed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="85eed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85eed-111">Não avaliado</span><span class="sxs-lookup"><span data-stu-id="85eed-111">notEvaluated</span></span>|<span data-ttu-id="85eed-112">,0</span><span class="sxs-lookup"><span data-stu-id="85eed-112">0</span></span>|<span data-ttu-id="85eed-113">Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85eed-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="85eed-114">falhou</span><span class="sxs-lookup"><span data-stu-id="85eed-114">failed</span></span>|<span data-ttu-id="85eed-115">1 </span><span class="sxs-lookup"><span data-stu-id="85eed-115">1</span></span>|<span data-ttu-id="85eed-116">Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85eed-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="85eed-117">instalado</span><span class="sxs-lookup"><span data-stu-id="85eed-117">installing</span></span>|<span data-ttu-id="85eed-118">2 </span><span class="sxs-lookup"><span data-stu-id="85eed-118">2</span></span>|<span data-ttu-id="85eed-119">Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.</span><span class="sxs-lookup"><span data-stu-id="85eed-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="85eed-120">instalação</span><span class="sxs-lookup"><span data-stu-id="85eed-120">installed</span></span>|<span data-ttu-id="85eed-121">3 </span><span class="sxs-lookup"><span data-stu-id="85eed-121">3</span></span>|<span data-ttu-id="85eed-122">Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="85eed-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="85eed-123">deleta</span><span class="sxs-lookup"><span data-stu-id="85eed-123">deleting</span></span>|<span data-ttu-id="85eed-124">4 </span><span class="sxs-lookup"><span data-stu-id="85eed-124">4</span></span>|<span data-ttu-id="85eed-125">Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85eed-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="85eed-126">erro</span><span class="sxs-lookup"><span data-stu-id="85eed-126">error</span></span>|<span data-ttu-id="85eed-127">5 </span><span class="sxs-lookup"><span data-stu-id="85eed-127">5</span></span>|<span data-ttu-id="85eed-128">Designa que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="85eed-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="85eed-129">deleted</span><span class="sxs-lookup"><span data-stu-id="85eed-129">deleted</span></span>|<span data-ttu-id="85eed-130">6 </span><span class="sxs-lookup"><span data-stu-id="85eed-130">6</span></span>|<span data-ttu-id="85eed-131">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85eed-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="85eed-132">removedByUser</span><span class="sxs-lookup"><span data-stu-id="85eed-132">removedByUser</span></span>|<span data-ttu-id="85eed-133">7 </span><span class="sxs-lookup"><span data-stu-id="85eed-133">7</span></span>|<span data-ttu-id="85eed-134">Designa que o perfil foi removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="85eed-134">Designates that the profile is removed from the device by the user</span></span>|





