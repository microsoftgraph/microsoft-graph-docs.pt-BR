---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585359"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="4cf50-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="4cf50-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="4cf50-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4cf50-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf50-105">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="4cf50-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="4cf50-106">Membros</span><span class="sxs-lookup"><span data-stu-id="4cf50-106">Members</span></span>
|<span data-ttu-id="4cf50-107">Membro</span><span class="sxs-lookup"><span data-stu-id="4cf50-107">Member</span></span>|<span data-ttu-id="4cf50-108">Valor</span><span class="sxs-lookup"><span data-stu-id="4cf50-108">Value</span></span>|<span data-ttu-id="4cf50-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cf50-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf50-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="4cf50-110">unknown</span></span>|<span data-ttu-id="4cf50-111">,0</span><span class="sxs-lookup"><span data-stu-id="4cf50-111">0</span></span>|<span data-ttu-id="4cf50-112">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="4cf50-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="4cf50-113">userRegistrar</span><span class="sxs-lookup"><span data-stu-id="4cf50-113">userEnrollment</span></span>|<span data-ttu-id="4cf50-114">1</span><span class="sxs-lookup"><span data-stu-id="4cf50-114">1</span></span>|<span data-ttu-id="4cf50-115">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="4cf50-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="4cf50-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="4cf50-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="4cf50-117">duas</span><span class="sxs-lookup"><span data-stu-id="4cf50-117">2</span></span>|<span data-ttu-id="4cf50-118">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cf50-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="4cf50-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="4cf50-119">appleBulkWithUser</span></span>|<span data-ttu-id="4cf50-120">3D</span><span class="sxs-lookup"><span data-stu-id="4cf50-120">3</span></span>|<span data-ttu-id="4cf50-121">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4cf50-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="4cf50-122">(DEP, Apple conFigurator)</span><span class="sxs-lookup"><span data-stu-id="4cf50-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="4cf50-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="4cf50-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="4cf50-124">quatro</span><span class="sxs-lookup"><span data-stu-id="4cf50-124">4</span></span>|<span data-ttu-id="4cf50-125">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4cf50-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="4cf50-126">(DEP, Apple conFigurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="4cf50-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="4cf50-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="4cf50-127">windowsAzureADJoin</span></span>|<span data-ttu-id="4cf50-128">0,5</span><span class="sxs-lookup"><span data-stu-id="4cf50-128">5</span></span>|<span data-ttu-id="4cf50-129">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4cf50-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="4cf50-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="4cf50-130">windowsBulkUserless</span></span>|<span data-ttu-id="4cf50-131">6</span><span class="sxs-lookup"><span data-stu-id="4cf50-131">6</span></span>|<span data-ttu-id="4cf50-132">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="4cf50-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="4cf50-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="4cf50-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="4cf50-134">178</span><span class="sxs-lookup"><span data-stu-id="4cf50-134">7</span></span>|<span data-ttu-id="4cf50-135">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4cf50-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="4cf50-136">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="4cf50-136">(Add work account)</span></span>|
|<span data-ttu-id="4cf50-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="4cf50-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="4cf50-138">8</span><span class="sxs-lookup"><span data-stu-id="4cf50-138">8</span></span>|<span data-ttu-id="4cf50-139">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4cf50-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="4cf50-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="4cf50-140">windowsCoManagement</span></span>|<span data-ttu-id="4cf50-141">241</span><span class="sxs-lookup"><span data-stu-id="4cf50-141">9</span></span>|<span data-ttu-id="4cf50-142">Co-gerenciamento de interGestão do Windows 10 disparado por autoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="4cf50-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



