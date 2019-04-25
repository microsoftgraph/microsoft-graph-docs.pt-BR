---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524586"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="a2da1-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a2da1-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="a2da1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2da1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2da1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2da1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2da1-106">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a2da1-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="a2da1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a2da1-107">Members</span></span>
|<span data-ttu-id="a2da1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a2da1-108">Member</span></span>|<span data-ttu-id="a2da1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a2da1-109">Value</span></span>|<span data-ttu-id="a2da1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2da1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2da1-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a2da1-111">unknown</span></span>|<span data-ttu-id="a2da1-112">,0</span><span class="sxs-lookup"><span data-stu-id="a2da1-112">0</span></span>|<span data-ttu-id="a2da1-113">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="a2da1-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="a2da1-114">userRegistrar</span><span class="sxs-lookup"><span data-stu-id="a2da1-114">userEnrollment</span></span>|<span data-ttu-id="a2da1-115">1 </span><span class="sxs-lookup"><span data-stu-id="a2da1-115">1</span></span>|<span data-ttu-id="a2da1-116">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="a2da1-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="a2da1-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="a2da1-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="a2da1-118">2 </span><span class="sxs-lookup"><span data-stu-id="a2da1-118">2</span></span>|<span data-ttu-id="a2da1-119">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2da1-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="a2da1-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="a2da1-120">appleBulkWithUser</span></span>|<span data-ttu-id="a2da1-121">3 </span><span class="sxs-lookup"><span data-stu-id="a2da1-121">3</span></span>|<span data-ttu-id="a2da1-122">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2da1-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="a2da1-123">(DEP, Apple conFigurator)</span><span class="sxs-lookup"><span data-stu-id="a2da1-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="a2da1-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="a2da1-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="a2da1-125">4 </span><span class="sxs-lookup"><span data-stu-id="a2da1-125">4</span></span>|<span data-ttu-id="a2da1-126">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2da1-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="a2da1-127">(DEP, Apple conFigurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="a2da1-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="a2da1-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="a2da1-128">windowsAzureADJoin</span></span>|<span data-ttu-id="a2da1-129">5 </span><span class="sxs-lookup"><span data-stu-id="a2da1-129">5</span></span>|<span data-ttu-id="a2da1-130">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a2da1-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="a2da1-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="a2da1-131">windowsBulkUserless</span></span>|<span data-ttu-id="a2da1-132">6 </span><span class="sxs-lookup"><span data-stu-id="a2da1-132">6</span></span>|<span data-ttu-id="a2da1-133">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="a2da1-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="a2da1-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="a2da1-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="a2da1-135">7 </span><span class="sxs-lookup"><span data-stu-id="a2da1-135">7</span></span>|<span data-ttu-id="a2da1-136">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a2da1-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="a2da1-137">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="a2da1-137">(Add work account)</span></span>|
|<span data-ttu-id="a2da1-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="a2da1-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="a2da1-139">8 </span><span class="sxs-lookup"><span data-stu-id="a2da1-139">8</span></span>|<span data-ttu-id="a2da1-140">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a2da1-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="a2da1-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="a2da1-141">windowsCoManagement</span></span>|<span data-ttu-id="a2da1-142">9 </span><span class="sxs-lookup"><span data-stu-id="a2da1-142">9</span></span>|<span data-ttu-id="a2da1-143">Co-gerenciamento de interGestão do Windows 10 disparado por autoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="a2da1-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




