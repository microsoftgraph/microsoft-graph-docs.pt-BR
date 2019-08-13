---
title: tipo de enumeração deviceEnrollmentType
description: Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b53d279863ad3e17691b9e4d0397ba5f7d1b408
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372080"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="46d30-103">tipo de enumeração deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="46d30-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="46d30-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46d30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46d30-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46d30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46d30-106">Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46d30-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="46d30-107">Membros</span><span class="sxs-lookup"><span data-stu-id="46d30-107">Members</span></span>
|<span data-ttu-id="46d30-108">Membro</span><span class="sxs-lookup"><span data-stu-id="46d30-108">Member</span></span>|<span data-ttu-id="46d30-109">Valor</span><span class="sxs-lookup"><span data-stu-id="46d30-109">Value</span></span>|<span data-ttu-id="46d30-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46d30-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="46d30-111">unknown</span></span>|<span data-ttu-id="46d30-112">,0</span><span class="sxs-lookup"><span data-stu-id="46d30-112">0</span></span>|<span data-ttu-id="46d30-113">O valor padrão, o tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="46d30-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="46d30-114">userregistrar</span><span class="sxs-lookup"><span data-stu-id="46d30-114">userEnrollment</span></span>|<span data-ttu-id="46d30-115">1</span><span class="sxs-lookup"><span data-stu-id="46d30-115">1</span></span>|<span data-ttu-id="46d30-116">Registro controlado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="46d30-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="46d30-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="46d30-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="46d30-118">duas</span><span class="sxs-lookup"><span data-stu-id="46d30-118">2</span></span>|<span data-ttu-id="46d30-119">Registro de usuário com uma conta de Gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46d30-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="46d30-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="46d30-120">appleBulkWithUser</span></span>|<span data-ttu-id="46d30-121">3D</span><span class="sxs-lookup"><span data-stu-id="46d30-121">3</span></span>|<span data-ttu-id="46d30-122">Inscrição em massa da Apple com o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="46d30-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="46d30-123">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="46d30-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="46d30-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="46d30-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="46d30-125">quatro</span><span class="sxs-lookup"><span data-stu-id="46d30-125">4</span></span>|<span data-ttu-id="46d30-126">Inscrição em massa da Apple sem o desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="46d30-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="46d30-127">(DEP, Apple Configurator, configuração móvel)</span><span class="sxs-lookup"><span data-stu-id="46d30-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="46d30-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="46d30-128">windowsAzureADJoin</span></span>|<span data-ttu-id="46d30-129">0,5</span><span class="sxs-lookup"><span data-stu-id="46d30-129">5</span></span>|<span data-ttu-id="46d30-130">Ingressar no Azure AD do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="46d30-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="46d30-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="46d30-131">windowsBulkUserless</span></span>|<span data-ttu-id="46d30-132">6</span><span class="sxs-lookup"><span data-stu-id="46d30-132">6</span></span>|<span data-ttu-id="46d30-133">Registro em massa do Windows 10 através do ICD com o certificado.</span><span class="sxs-lookup"><span data-stu-id="46d30-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="46d30-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="46d30-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="46d30-135">178</span><span class="sxs-lookup"><span data-stu-id="46d30-135">7</span></span>|<span data-ttu-id="46d30-136">Registro automático do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="46d30-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="46d30-137">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="46d30-137">(Add work account)</span></span>|
|<span data-ttu-id="46d30-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="46d30-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="46d30-139">8 </span><span class="sxs-lookup"><span data-stu-id="46d30-139">8</span></span>|<span data-ttu-id="46d30-140">Ingresso no Azure AD em massa do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="46d30-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="46d30-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="46d30-141">windowsCoManagement</span></span>|<span data-ttu-id="46d30-142">9 </span><span class="sxs-lookup"><span data-stu-id="46d30-142">9</span></span>|<span data-ttu-id="46d30-143">Co-gerenciamento de intergestão do Windows 10 disparado por AutoPilot ou política de grupo.</span><span class="sxs-lookup"><span data-stu-id="46d30-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



