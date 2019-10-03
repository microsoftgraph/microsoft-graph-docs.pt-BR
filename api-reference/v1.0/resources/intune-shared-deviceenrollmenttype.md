---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae60fd6657cf902eb5bdd0f919d446527b00d9a9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368271"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="a40e0-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a40e0-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="a40e0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a40e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a40e0-105">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a40e0-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="a40e0-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a40e0-106">Members</span></span>
|<span data-ttu-id="a40e0-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a40e0-107">Member</span></span>|<span data-ttu-id="a40e0-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a40e0-108">Value</span></span>|<span data-ttu-id="a40e0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a40e0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a40e0-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a40e0-110">unknown</span></span>|<span data-ttu-id="a40e0-111">,0</span><span class="sxs-lookup"><span data-stu-id="a40e0-111">0</span></span>|<span data-ttu-id="a40e0-112">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="a40e0-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="a40e0-113">userregistrar</span><span class="sxs-lookup"><span data-stu-id="a40e0-113">userEnrollment</span></span>|<span data-ttu-id="a40e0-114">1</span><span class="sxs-lookup"><span data-stu-id="a40e0-114">1</span></span>|<span data-ttu-id="a40e0-115">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="a40e0-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="a40e0-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="a40e0-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="a40e0-117">duas</span><span class="sxs-lookup"><span data-stu-id="a40e0-117">2</span></span>|<span data-ttu-id="a40e0-118">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a40e0-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="a40e0-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="a40e0-119">appleBulkWithUser</span></span>|<span data-ttu-id="a40e0-120">3D</span><span class="sxs-lookup"><span data-stu-id="a40e0-120">3</span></span>|<span data-ttu-id="a40e0-121">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a40e0-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="a40e0-122">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="a40e0-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="a40e0-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="a40e0-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="a40e0-124">quatro</span><span class="sxs-lookup"><span data-stu-id="a40e0-124">4</span></span>|<span data-ttu-id="a40e0-125">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a40e0-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="a40e0-126">(DEP, Apple Configurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="a40e0-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="a40e0-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="a40e0-127">windowsAzureADJoin</span></span>|<span data-ttu-id="a40e0-128">0,5</span><span class="sxs-lookup"><span data-stu-id="a40e0-128">5</span></span>|<span data-ttu-id="a40e0-129">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a40e0-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="a40e0-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="a40e0-130">windowsBulkUserless</span></span>|<span data-ttu-id="a40e0-131">6</span><span class="sxs-lookup"><span data-stu-id="a40e0-131">6</span></span>|<span data-ttu-id="a40e0-132">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="a40e0-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="a40e0-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="a40e0-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="a40e0-134">178</span><span class="sxs-lookup"><span data-stu-id="a40e0-134">7</span></span>|<span data-ttu-id="a40e0-135">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a40e0-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="a40e0-136">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="a40e0-136">(Add work account)</span></span>|
|<span data-ttu-id="a40e0-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="a40e0-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="a40e0-138">8 </span><span class="sxs-lookup"><span data-stu-id="a40e0-138">8</span></span>|<span data-ttu-id="a40e0-139">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a40e0-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="a40e0-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="a40e0-140">windowsCoManagement</span></span>|<span data-ttu-id="a40e0-141">9 </span><span class="sxs-lookup"><span data-stu-id="a40e0-141">9</span></span>|<span data-ttu-id="a40e0-142">Co-gerenciamento de intergestão do Windows 10 disparado por AutoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a40e0-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




