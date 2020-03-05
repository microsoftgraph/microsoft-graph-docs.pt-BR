---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1df6e595af1592487130cd2ef3a26c15397ce846
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447854"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="e84eb-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="e84eb-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="e84eb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e84eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e84eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e84eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e84eb-106">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e84eb-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="e84eb-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e84eb-107">Members</span></span>
|<span data-ttu-id="e84eb-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e84eb-108">Member</span></span>|<span data-ttu-id="e84eb-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e84eb-109">Value</span></span>|<span data-ttu-id="e84eb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e84eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e84eb-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e84eb-111">unknown</span></span>|<span data-ttu-id="e84eb-112">,0</span><span class="sxs-lookup"><span data-stu-id="e84eb-112">0</span></span>|<span data-ttu-id="e84eb-113">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="e84eb-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="e84eb-114">userregistrar</span><span class="sxs-lookup"><span data-stu-id="e84eb-114">userEnrollment</span></span>|<span data-ttu-id="e84eb-115">1 </span><span class="sxs-lookup"><span data-stu-id="e84eb-115">1</span></span>|<span data-ttu-id="e84eb-116">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="e84eb-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="e84eb-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="e84eb-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="e84eb-118">2 </span><span class="sxs-lookup"><span data-stu-id="e84eb-118">2</span></span>|<span data-ttu-id="e84eb-119">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e84eb-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="e84eb-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="e84eb-120">appleBulkWithUser</span></span>|<span data-ttu-id="e84eb-121">3 </span><span class="sxs-lookup"><span data-stu-id="e84eb-121">3</span></span>|<span data-ttu-id="e84eb-122">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e84eb-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="e84eb-123">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="e84eb-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="e84eb-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="e84eb-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="e84eb-125">4 </span><span class="sxs-lookup"><span data-stu-id="e84eb-125">4</span></span>|<span data-ttu-id="e84eb-126">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e84eb-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="e84eb-127">(DEP, Apple Configurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="e84eb-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="e84eb-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="e84eb-128">windowsAzureADJoin</span></span>|<span data-ttu-id="e84eb-129">5 </span><span class="sxs-lookup"><span data-stu-id="e84eb-129">5</span></span>|<span data-ttu-id="e84eb-130">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e84eb-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="e84eb-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="e84eb-131">windowsBulkUserless</span></span>|<span data-ttu-id="e84eb-132">6 </span><span class="sxs-lookup"><span data-stu-id="e84eb-132">6</span></span>|<span data-ttu-id="e84eb-133">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="e84eb-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="e84eb-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="e84eb-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="e84eb-135">7 </span><span class="sxs-lookup"><span data-stu-id="e84eb-135">7</span></span>|<span data-ttu-id="e84eb-136">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e84eb-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="e84eb-137">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="e84eb-137">(Add work account)</span></span>|
|<span data-ttu-id="e84eb-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="e84eb-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="e84eb-139">8 </span><span class="sxs-lookup"><span data-stu-id="e84eb-139">8</span></span>|<span data-ttu-id="e84eb-140">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e84eb-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="e84eb-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="e84eb-141">windowsCoManagement</span></span>|<span data-ttu-id="e84eb-142">9 </span><span class="sxs-lookup"><span data-stu-id="e84eb-142">9</span></span>|<span data-ttu-id="e84eb-143">Co-gerenciamento de intergestão do Windows 10 disparado por AutoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="e84eb-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




