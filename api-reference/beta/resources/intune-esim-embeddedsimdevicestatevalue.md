---
title: tipo de enum embeddedSIMDeviceStateValue
description: Descreve os diversos estados de um código de ativação SIM incorporado.
author: tfitzmac
ms.openlocfilehash: 51e550669d9cd29d7d5bb246fe2cba017b02187c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320591"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="adcbe-103">tipo de enum embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="adcbe-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="adcbe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="adcbe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adcbe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="adcbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adcbe-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="adcbe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adcbe-107">Descreve os diversos estados de um código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="adcbe-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="adcbe-108">Membros</span><span class="sxs-lookup"><span data-stu-id="adcbe-108">Members</span></span>
|<span data-ttu-id="adcbe-109">Membro</span><span class="sxs-lookup"><span data-stu-id="adcbe-109">Member</span></span>|<span data-ttu-id="adcbe-110">Valor</span><span class="sxs-lookup"><span data-stu-id="adcbe-110">Value</span></span>|<span data-ttu-id="adcbe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="adcbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adcbe-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="adcbe-112">notEvaluated</span></span>|<span data-ttu-id="adcbe-113">0</span><span class="sxs-lookup"><span data-stu-id="adcbe-113">0</span></span>|<span data-ttu-id="adcbe-114">Designa que o código de ativação SIM incorporado é gratuito e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adcbe-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="adcbe-115">Falha</span><span class="sxs-lookup"><span data-stu-id="adcbe-115">failed</span></span>|<span data-ttu-id="adcbe-116">1</span><span class="sxs-lookup"><span data-stu-id="adcbe-116">1</span></span>|<span data-ttu-id="adcbe-117">Designa que Intune Service falhou ao entregar esse perfil para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adcbe-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="adcbe-118">Instalando</span><span class="sxs-lookup"><span data-stu-id="adcbe-118">installing</span></span>|<span data-ttu-id="adcbe-119">2</span><span class="sxs-lookup"><span data-stu-id="adcbe-119">2</span></span>|<span data-ttu-id="adcbe-120">Designa que o código de ativação SIM incorporado tenha sido atribuído a um dispositivo e o dispositivo está instalando o token.</span><span class="sxs-lookup"><span data-stu-id="adcbe-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="adcbe-121">instalado</span><span class="sxs-lookup"><span data-stu-id="adcbe-121">installed</span></span>|<span data-ttu-id="adcbe-122">3</span><span class="sxs-lookup"><span data-stu-id="adcbe-122">3</span></span>|<span data-ttu-id="adcbe-123">Designa se o código de ativação SIM incorporado foi instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="adcbe-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="adcbe-124">excluindo</span><span class="sxs-lookup"><span data-stu-id="adcbe-124">deleting</span></span>|<span data-ttu-id="adcbe-125">4</span><span class="sxs-lookup"><span data-stu-id="adcbe-125">4</span></span>|<span data-ttu-id="adcbe-126">Designa Intune Service está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adcbe-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="adcbe-127">erro</span><span class="sxs-lookup"><span data-stu-id="adcbe-127">error</span></span>|<span data-ttu-id="adcbe-128">5</span><span class="sxs-lookup"><span data-stu-id="adcbe-128">5</span></span>|<span data-ttu-id="adcbe-129">Designa o que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="adcbe-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="adcbe-130">deleted</span><span class="sxs-lookup"><span data-stu-id="adcbe-130">deleted</span></span>|<span data-ttu-id="adcbe-131">6</span><span class="sxs-lookup"><span data-stu-id="adcbe-131">6</span></span>|<span data-ttu-id="adcbe-132">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="adcbe-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="adcbe-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="adcbe-133">removedByUser</span></span>|<span data-ttu-id="adcbe-134">7</span><span class="sxs-lookup"><span data-stu-id="adcbe-134">7</span></span>|<span data-ttu-id="adcbe-135">Designa que o perfil é removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="adcbe-135">Designates that the profile is removed from the device by the user</span></span>|





