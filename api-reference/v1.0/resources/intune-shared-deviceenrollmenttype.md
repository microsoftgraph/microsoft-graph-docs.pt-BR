---
title: Tipo de número deviceEnrollmentType
description: Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732223"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="f6ba4-103">Tipo de número deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="f6ba4-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="f6ba4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6ba4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6ba4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ba4-106">Possíveis maneiras de adicionar um dispositivo móvel ao gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="f6ba4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f6ba4-107">Members</span></span>
|<span data-ttu-id="f6ba4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f6ba4-108">Member</span></span>|<span data-ttu-id="f6ba4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f6ba4-109">Value</span></span>|<span data-ttu-id="f6ba4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ba4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ba4-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f6ba4-111">unknown</span></span>|<span data-ttu-id="f6ba4-112">0</span><span class="sxs-lookup"><span data-stu-id="f6ba4-112">0</span></span>|<span data-ttu-id="f6ba4-113">Valor padrão, tipo de registro não coletado.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="f6ba4-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="f6ba4-114">userEnrollment</span></span>|<span data-ttu-id="f6ba4-115">1</span><span class="sxs-lookup"><span data-stu-id="f6ba4-115">1</span></span>|<span data-ttu-id="f6ba4-116">Registro orientado pelo usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="f6ba4-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="f6ba4-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="f6ba4-118">2</span><span class="sxs-lookup"><span data-stu-id="f6ba4-118">2</span></span>|<span data-ttu-id="f6ba4-119">Registro de usuário com uma conta do gerenciador de registro de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="f6ba4-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="f6ba4-120">appleBulkWithUser</span></span>|<span data-ttu-id="f6ba4-121">3</span><span class="sxs-lookup"><span data-stu-id="f6ba4-121">3</span></span>|<span data-ttu-id="f6ba4-122">Registro em massa da Apple com desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="f6ba4-123">(DEP, Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="f6ba4-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="f6ba4-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="f6ba4-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="f6ba4-125">4 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-125">4</span></span>|<span data-ttu-id="f6ba4-126">Registro em massa da Apple sem desafio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="f6ba4-127">(DEP, Apple Configurator, Mobile Config)</span><span class="sxs-lookup"><span data-stu-id="f6ba4-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="f6ba4-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="f6ba4-128">windowsAzureADJoin</span></span>|<span data-ttu-id="f6ba4-129">5 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-129">5</span></span>|<span data-ttu-id="f6ba4-130">Windows 10 Ingressar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="f6ba4-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="f6ba4-131">windowsBulkUserless</span></span>|<span data-ttu-id="f6ba4-132">6 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-132">6</span></span>|<span data-ttu-id="f6ba4-133">Windows 10 Registro em massa por meio do ICD com certificado.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="f6ba4-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="f6ba4-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="f6ba4-135">7 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-135">7</span></span>|<span data-ttu-id="f6ba4-136">Windows 10 registro automático.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="f6ba4-137">(Adicionar conta de trabalho)</span><span class="sxs-lookup"><span data-stu-id="f6ba4-137">(Add work account)</span></span>|
|<span data-ttu-id="f6ba4-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="f6ba4-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="f6ba4-139">8 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-139">8</span></span>|<span data-ttu-id="f6ba4-140">Windows 10 participar em massa do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="f6ba4-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="f6ba4-141">windowsCoManagement</span></span>|<span data-ttu-id="f6ba4-142">9 </span><span class="sxs-lookup"><span data-stu-id="f6ba4-142">9</span></span>|<span data-ttu-id="f6ba4-143">Windows 10 Co-Management acionado pelo AutoPilot ou Pela Política de Grupo.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|









