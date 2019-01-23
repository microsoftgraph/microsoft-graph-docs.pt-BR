---
title: tipo de enum deviceEnrollmentType
description: Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399287"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="ec215-103">tipo de enum deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ec215-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="ec215-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec215-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec215-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec215-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec215-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ec215-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec215-107">Maneiras possíveis de adição de um dispositivo móvel gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ec215-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="ec215-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ec215-108">Members</span></span>
|<span data-ttu-id="ec215-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ec215-109">Member</span></span>|<span data-ttu-id="ec215-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ec215-110">Value</span></span>|<span data-ttu-id="ec215-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec215-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec215-112">unknown</span><span class="sxs-lookup"><span data-stu-id="ec215-112">unknown</span></span>|<span data-ttu-id="ec215-113">0</span><span class="sxs-lookup"><span data-stu-id="ec215-113">0</span></span>|<span data-ttu-id="ec215-114">O valor padrão, tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="ec215-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="ec215-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="ec215-115">userEnrollment</span></span>|<span data-ttu-id="ec215-116">1</span><span class="sxs-lookup"><span data-stu-id="ec215-116">1</span></span>|<span data-ttu-id="ec215-117">Inscrição do orientado por usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="ec215-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="ec215-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="ec215-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="ec215-119">2</span><span class="sxs-lookup"><span data-stu-id="ec215-119">2</span></span>|<span data-ttu-id="ec215-120">Inscrição do usuário com uma conta de Gerenciador de inscrição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec215-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="ec215-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="ec215-121">appleBulkWithUser</span></span>|<span data-ttu-id="ec215-122">3</span><span class="sxs-lookup"><span data-stu-id="ec215-122">3</span></span>|<span data-ttu-id="ec215-123">Inscrição do Apple em massa com o desafio de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec215-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="ec215-124">Configurador Apple (DEP)</span><span class="sxs-lookup"><span data-stu-id="ec215-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="ec215-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="ec215-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="ec215-126">4</span><span class="sxs-lookup"><span data-stu-id="ec215-126">4</span></span>|<span data-ttu-id="ec215-127">Inscrição do Apple em massa sem o desafio de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec215-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="ec215-128">(DEP, Apple configurador, móvel Config)</span><span class="sxs-lookup"><span data-stu-id="ec215-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="ec215-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="ec215-129">windowsAzureADJoin</span></span>|<span data-ttu-id="ec215-130">5</span><span class="sxs-lookup"><span data-stu-id="ec215-130">5</span></span>|<span data-ttu-id="ec215-131">Windows Azure AD de 10 ingressam.</span><span class="sxs-lookup"><span data-stu-id="ec215-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="ec215-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="ec215-132">windowsBulkUserless</span></span>|<span data-ttu-id="ec215-133">6</span><span class="sxs-lookup"><span data-stu-id="ec215-133">6</span></span>|<span data-ttu-id="ec215-134">Inscrição em massa de 10 Windows por meio de ICD com certificado.</span><span class="sxs-lookup"><span data-stu-id="ec215-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="ec215-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="ec215-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="ec215-136">7</span><span class="sxs-lookup"><span data-stu-id="ec215-136">7</span></span>|<span data-ttu-id="ec215-137">Inscrição automática do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="ec215-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="ec215-138">(Adicionar a conta do trabalho)</span><span class="sxs-lookup"><span data-stu-id="ec215-138">(Add work account)</span></span>|
|<span data-ttu-id="ec215-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="ec215-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="ec215-140">8</span><span class="sxs-lookup"><span data-stu-id="ec215-140">8</span></span>|<span data-ttu-id="ec215-141">Windows 10 em massa ingressar do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ec215-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="ec215-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="ec215-142">windowsCoManagement</span></span>|<span data-ttu-id="ec215-143">9</span><span class="sxs-lookup"><span data-stu-id="ec215-143">9</span></span>|<span data-ttu-id="ec215-144">Gerenciamento de colegas de 10 Windows acionadas por piloto automático ou a diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="ec215-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




