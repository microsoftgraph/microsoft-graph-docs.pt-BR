---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ae3edcb1d6411e889381c2171f0daeb1cbcc528
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996138"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="903fa-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="903fa-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="903fa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="903fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="903fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="903fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="903fa-106">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="903fa-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="903fa-107">Membros</span><span class="sxs-lookup"><span data-stu-id="903fa-107">Members</span></span>
|<span data-ttu-id="903fa-108">Membro</span><span class="sxs-lookup"><span data-stu-id="903fa-108">Member</span></span>|<span data-ttu-id="903fa-109">Valor</span><span class="sxs-lookup"><span data-stu-id="903fa-109">Value</span></span>|<span data-ttu-id="903fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="903fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="903fa-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="903fa-111">unknown</span></span>|<span data-ttu-id="903fa-112">,0</span><span class="sxs-lookup"><span data-stu-id="903fa-112">0</span></span>|<span data-ttu-id="903fa-113">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="903fa-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="903fa-114">userregistrar</span><span class="sxs-lookup"><span data-stu-id="903fa-114">userEnrollment</span></span>|<span data-ttu-id="903fa-115">1</span><span class="sxs-lookup"><span data-stu-id="903fa-115">1</span></span>|<span data-ttu-id="903fa-116">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="903fa-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="903fa-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="903fa-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="903fa-118">duas</span><span class="sxs-lookup"><span data-stu-id="903fa-118">2</span></span>|<span data-ttu-id="903fa-119">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="903fa-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="903fa-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="903fa-120">appleBulkWithUser</span></span>|<span data-ttu-id="903fa-121">3D</span><span class="sxs-lookup"><span data-stu-id="903fa-121">3</span></span>|<span data-ttu-id="903fa-122">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="903fa-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="903fa-123">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="903fa-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="903fa-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="903fa-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="903fa-125">quatro</span><span class="sxs-lookup"><span data-stu-id="903fa-125">4</span></span>|<span data-ttu-id="903fa-126">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="903fa-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="903fa-127">(DEP, Apple Configurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="903fa-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="903fa-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="903fa-128">windowsAzureADJoin</span></span>|<span data-ttu-id="903fa-129">0,5</span><span class="sxs-lookup"><span data-stu-id="903fa-129">5</span></span>|<span data-ttu-id="903fa-130">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="903fa-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="903fa-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="903fa-131">windowsBulkUserless</span></span>|<span data-ttu-id="903fa-132">6</span><span class="sxs-lookup"><span data-stu-id="903fa-132">6</span></span>|<span data-ttu-id="903fa-133">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="903fa-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="903fa-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="903fa-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="903fa-135">178</span><span class="sxs-lookup"><span data-stu-id="903fa-135">7</span></span>|<span data-ttu-id="903fa-136">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="903fa-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="903fa-137">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="903fa-137">(Add work account)</span></span>|
|<span data-ttu-id="903fa-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="903fa-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="903fa-139">8 </span><span class="sxs-lookup"><span data-stu-id="903fa-139">8</span></span>|<span data-ttu-id="903fa-140">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="903fa-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="903fa-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="903fa-141">windowsCoManagement</span></span>|<span data-ttu-id="903fa-142">9 </span><span class="sxs-lookup"><span data-stu-id="903fa-142">9</span></span>|<span data-ttu-id="903fa-143">Co-gerenciamento de intergestão do Windows 10 disparado por AutoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="903fa-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





