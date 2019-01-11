---
title: tipo de enum embeddedSIMDeviceStateValue
description: Descreve os diversos estados de um código de ativação SIM incorporado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3974c0df65ef9f59242f390b7166e11c3e0c592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886055"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="f4a8a-103">tipo de enum embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="f4a8a-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="f4a8a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4a8a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4a8a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4a8a-107">Descreve os diversos estados de um código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="f4a8a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f4a8a-108">Members</span></span>
|<span data-ttu-id="f4a8a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f4a8a-109">Member</span></span>|<span data-ttu-id="f4a8a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f4a8a-110">Value</span></span>|<span data-ttu-id="f4a8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a8a-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="f4a8a-112">notEvaluated</span></span>|<span data-ttu-id="f4a8a-113">0</span><span class="sxs-lookup"><span data-stu-id="f4a8a-113">0</span></span>|<span data-ttu-id="f4a8a-114">Designa que o código de ativação SIM incorporado é gratuito e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="f4a8a-115">Falha</span><span class="sxs-lookup"><span data-stu-id="f4a8a-115">failed</span></span>|<span data-ttu-id="f4a8a-116">1</span><span class="sxs-lookup"><span data-stu-id="f4a8a-116">1</span></span>|<span data-ttu-id="f4a8a-117">Designa que Intune Service falhou ao entregar esse perfil para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="f4a8a-118">Instalando</span><span class="sxs-lookup"><span data-stu-id="f4a8a-118">installing</span></span>|<span data-ttu-id="f4a8a-119">2</span><span class="sxs-lookup"><span data-stu-id="f4a8a-119">2</span></span>|<span data-ttu-id="f4a8a-120">Designa que o código de ativação SIM incorporado tenha sido atribuído a um dispositivo e o dispositivo está instalando o token.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="f4a8a-121">instalado</span><span class="sxs-lookup"><span data-stu-id="f4a8a-121">installed</span></span>|<span data-ttu-id="f4a8a-122">3</span><span class="sxs-lookup"><span data-stu-id="f4a8a-122">3</span></span>|<span data-ttu-id="f4a8a-123">Designa se o código de ativação SIM incorporado foi instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="f4a8a-124">excluindo</span><span class="sxs-lookup"><span data-stu-id="f4a8a-124">deleting</span></span>|<span data-ttu-id="f4a8a-125">4</span><span class="sxs-lookup"><span data-stu-id="f4a8a-125">4</span></span>|<span data-ttu-id="f4a8a-126">Designa Intune Service está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="f4a8a-127">erro</span><span class="sxs-lookup"><span data-stu-id="f4a8a-127">error</span></span>|<span data-ttu-id="f4a8a-128">5</span><span class="sxs-lookup"><span data-stu-id="f4a8a-128">5</span></span>|<span data-ttu-id="f4a8a-129">Designa o que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="f4a8a-130">deleted</span><span class="sxs-lookup"><span data-stu-id="f4a8a-130">deleted</span></span>|<span data-ttu-id="f4a8a-131">6</span><span class="sxs-lookup"><span data-stu-id="f4a8a-131">6</span></span>|<span data-ttu-id="f4a8a-132">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4a8a-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="f4a8a-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="f4a8a-133">removedByUser</span></span>|<span data-ttu-id="f4a8a-134">7</span><span class="sxs-lookup"><span data-stu-id="f4a8a-134">7</span></span>|<span data-ttu-id="f4a8a-135">Designa que o perfil é removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f4a8a-135">Designates that the profile is removed from the device by the user</span></span>|





