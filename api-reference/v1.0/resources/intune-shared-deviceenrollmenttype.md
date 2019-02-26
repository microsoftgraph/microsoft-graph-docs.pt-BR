---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261961"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="cf025-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="cf025-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="cf025-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf025-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf025-105">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="cf025-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="cf025-106">Membros</span><span class="sxs-lookup"><span data-stu-id="cf025-106">Members</span></span>
|<span data-ttu-id="cf025-107">Membro</span><span class="sxs-lookup"><span data-stu-id="cf025-107">Member</span></span>|<span data-ttu-id="cf025-108">Valor</span><span class="sxs-lookup"><span data-stu-id="cf025-108">Value</span></span>|<span data-ttu-id="cf025-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf025-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf025-110">unknown</span><span class="sxs-lookup"><span data-stu-id="cf025-110">unknown</span></span>|<span data-ttu-id="cf025-111">,0</span><span class="sxs-lookup"><span data-stu-id="cf025-111">0</span></span>|<span data-ttu-id="cf025-112">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="cf025-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="cf025-113">userRegistrar</span><span class="sxs-lookup"><span data-stu-id="cf025-113">userEnrollment</span></span>|<span data-ttu-id="cf025-114">1</span><span class="sxs-lookup"><span data-stu-id="cf025-114">1</span></span>|<span data-ttu-id="cf025-115">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="cf025-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="cf025-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="cf025-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="cf025-117">duas</span><span class="sxs-lookup"><span data-stu-id="cf025-117">2</span></span>|<span data-ttu-id="cf025-118">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf025-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="cf025-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="cf025-119">appleBulkWithUser</span></span>|<span data-ttu-id="cf025-120">3D</span><span class="sxs-lookup"><span data-stu-id="cf025-120">3</span></span>|<span data-ttu-id="cf025-121">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf025-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="cf025-122">(DEP, Apple conFigurator)</span><span class="sxs-lookup"><span data-stu-id="cf025-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="cf025-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="cf025-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="cf025-124">quatro</span><span class="sxs-lookup"><span data-stu-id="cf025-124">4</span></span>|<span data-ttu-id="cf025-125">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cf025-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="cf025-126">(DEP, Apple conFigurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="cf025-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="cf025-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="cf025-127">windowsAzureADJoin</span></span>|<span data-ttu-id="cf025-128">0,5</span><span class="sxs-lookup"><span data-stu-id="cf025-128">5</span></span>|<span data-ttu-id="cf025-129">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="cf025-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="cf025-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="cf025-130">windowsBulkUserless</span></span>|<span data-ttu-id="cf025-131">6</span><span class="sxs-lookup"><span data-stu-id="cf025-131">6</span></span>|<span data-ttu-id="cf025-132">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="cf025-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="cf025-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="cf025-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="cf025-134">178</span><span class="sxs-lookup"><span data-stu-id="cf025-134">7</span></span>|<span data-ttu-id="cf025-135">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="cf025-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="cf025-136">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="cf025-136">(Add work account)</span></span>|
|<span data-ttu-id="cf025-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="cf025-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="cf025-138">8</span><span class="sxs-lookup"><span data-stu-id="cf025-138">8</span></span>|<span data-ttu-id="cf025-139">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="cf025-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="cf025-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="cf025-140">windowsCoManagement</span></span>|<span data-ttu-id="cf025-141">241</span><span class="sxs-lookup"><span data-stu-id="cf025-141">9</span></span>|<span data-ttu-id="cf025-142">Co-gerenciamento de interGestão do Windows 10 disparado por autoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="cf025-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



