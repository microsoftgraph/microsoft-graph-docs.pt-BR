---
title: tipo de enum embeddedSIMDeviceStateValue
description: Descreve os diversos estados de um código de ativação SIM incorporado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421323"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="6c80c-103">tipo de enum embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="6c80c-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="6c80c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c80c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c80c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c80c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c80c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c80c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c80c-107">Descreve os diversos estados de um código de ativação SIM incorporado.</span><span class="sxs-lookup"><span data-stu-id="6c80c-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="6c80c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6c80c-108">Members</span></span>
|<span data-ttu-id="6c80c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6c80c-109">Member</span></span>|<span data-ttu-id="6c80c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6c80c-110">Value</span></span>|<span data-ttu-id="6c80c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c80c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c80c-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="6c80c-112">notEvaluated</span></span>|<span data-ttu-id="6c80c-113">0</span><span class="sxs-lookup"><span data-stu-id="6c80c-113">0</span></span>|<span data-ttu-id="6c80c-114">Designa que o código de ativação SIM incorporado é gratuito e disponível para ser atribuído a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c80c-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="6c80c-115">Falha</span><span class="sxs-lookup"><span data-stu-id="6c80c-115">failed</span></span>|<span data-ttu-id="6c80c-116">1</span><span class="sxs-lookup"><span data-stu-id="6c80c-116">1</span></span>|<span data-ttu-id="6c80c-117">Designa que Intune Service falhou ao entregar esse perfil para um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c80c-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="6c80c-118">Instalando</span><span class="sxs-lookup"><span data-stu-id="6c80c-118">installing</span></span>|<span data-ttu-id="6c80c-119">2</span><span class="sxs-lookup"><span data-stu-id="6c80c-119">2</span></span>|<span data-ttu-id="6c80c-120">Designa que o código de ativação SIM incorporado tenha sido atribuído a um dispositivo e o dispositivo está instalando o token.</span><span class="sxs-lookup"><span data-stu-id="6c80c-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="6c80c-121">instalado</span><span class="sxs-lookup"><span data-stu-id="6c80c-121">installed</span></span>|<span data-ttu-id="6c80c-122">3</span><span class="sxs-lookup"><span data-stu-id="6c80c-122">3</span></span>|<span data-ttu-id="6c80c-123">Designa se o código de ativação SIM incorporado foi instalado com êxito no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="6c80c-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="6c80c-124">excluindo</span><span class="sxs-lookup"><span data-stu-id="6c80c-124">deleting</span></span>|<span data-ttu-id="6c80c-125">4</span><span class="sxs-lookup"><span data-stu-id="6c80c-125">4</span></span>|<span data-ttu-id="6c80c-126">Designa Intune Service está tentando excluir o perfil do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c80c-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="6c80c-127">erro</span><span class="sxs-lookup"><span data-stu-id="6c80c-127">error</span></span>|<span data-ttu-id="6c80c-128">5</span><span class="sxs-lookup"><span data-stu-id="6c80c-128">5</span></span>|<span data-ttu-id="6c80c-129">Designa o que há um erro com esse perfil.</span><span class="sxs-lookup"><span data-stu-id="6c80c-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="6c80c-130">deleted</span><span class="sxs-lookup"><span data-stu-id="6c80c-130">deleted</span></span>|<span data-ttu-id="6c80c-131">6</span><span class="sxs-lookup"><span data-stu-id="6c80c-131">6</span></span>|<span data-ttu-id="6c80c-132">Designa que o perfil é excluído do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c80c-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="6c80c-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="6c80c-133">removedByUser</span></span>|<span data-ttu-id="6c80c-134">7</span><span class="sxs-lookup"><span data-stu-id="6c80c-134">7</span></span>|<span data-ttu-id="6c80c-135">Designa que o perfil é removido do dispositivo pelo usuário</span><span class="sxs-lookup"><span data-stu-id="6c80c-135">Designates that the profile is removed from the device by the user</span></span>|




