---
title: tipo de enum deviceEnrollmentType
description: Maneiras possíveis de adição de um dispositivo móvel gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987752"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="473b9-103">tipo de enum deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="473b9-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="473b9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="473b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="473b9-105">Maneiras possíveis de adição de um dispositivo móvel gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="473b9-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="473b9-106">Membros</span><span class="sxs-lookup"><span data-stu-id="473b9-106">Members</span></span>
|<span data-ttu-id="473b9-107">Membro</span><span class="sxs-lookup"><span data-stu-id="473b9-107">Member</span></span>|<span data-ttu-id="473b9-108">Valor</span><span class="sxs-lookup"><span data-stu-id="473b9-108">Value</span></span>|<span data-ttu-id="473b9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="473b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="473b9-110">unknown</span><span class="sxs-lookup"><span data-stu-id="473b9-110">unknown</span></span>|<span data-ttu-id="473b9-111">0</span><span class="sxs-lookup"><span data-stu-id="473b9-111">0</span></span>|<span data-ttu-id="473b9-112">O valor padrão, tipo de registro não foi coletado.</span><span class="sxs-lookup"><span data-stu-id="473b9-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="473b9-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="473b9-113">userEnrollment</span></span>|<span data-ttu-id="473b9-114">1</span><span class="sxs-lookup"><span data-stu-id="473b9-114">1</span></span>|<span data-ttu-id="473b9-115">Inscrição do orientado por usuário por meio do canal BYOD.</span><span class="sxs-lookup"><span data-stu-id="473b9-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="473b9-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="473b9-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="473b9-117">2</span><span class="sxs-lookup"><span data-stu-id="473b9-117">2</span></span>|<span data-ttu-id="473b9-118">Inscrição do usuário com uma conta de Gerenciador de inscrição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="473b9-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="473b9-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="473b9-119">appleBulkWithUser</span></span>|<span data-ttu-id="473b9-120">3</span><span class="sxs-lookup"><span data-stu-id="473b9-120">3</span></span>|<span data-ttu-id="473b9-121">Inscrição do Apple em massa com o desafio de usuário (DEP, Apple configurador).</span><span class="sxs-lookup"><span data-stu-id="473b9-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="473b9-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="473b9-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="473b9-123">4</span><span class="sxs-lookup"><span data-stu-id="473b9-123">4</span></span>|<span data-ttu-id="473b9-124">Inscrição do Apple em massa sem o desafio de usuário (DEP, Apple configurador, Mobile Config).</span><span class="sxs-lookup"><span data-stu-id="473b9-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="473b9-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="473b9-125">windowsAzureADJoin</span></span>|<span data-ttu-id="473b9-126">5</span><span class="sxs-lookup"><span data-stu-id="473b9-126">5</span></span>|<span data-ttu-id="473b9-127">Windows Azure AD de 10 ingressam.</span><span class="sxs-lookup"><span data-stu-id="473b9-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="473b9-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="473b9-128">windowsBulkUserless</span></span>|<span data-ttu-id="473b9-129">6</span><span class="sxs-lookup"><span data-stu-id="473b9-129">6</span></span>|<span data-ttu-id="473b9-130">Inscrição em massa de 10 Windows por meio de ICD com certificado.</span><span class="sxs-lookup"><span data-stu-id="473b9-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="473b9-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="473b9-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="473b9-132">7</span><span class="sxs-lookup"><span data-stu-id="473b9-132">7</span></span>|<span data-ttu-id="473b9-133">Inscrição automática do Windows 10.</span><span class="sxs-lookup"><span data-stu-id="473b9-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="473b9-134">(Adicionar a conta do trabalho)</span><span class="sxs-lookup"><span data-stu-id="473b9-134">(Add work account)</span></span>|
|<span data-ttu-id="473b9-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="473b9-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="473b9-136">8</span><span class="sxs-lookup"><span data-stu-id="473b9-136">8</span></span>|<span data-ttu-id="473b9-137">Windows 10 em massa ingressar do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="473b9-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="473b9-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="473b9-138">windowsCoManagement</span></span>|<span data-ttu-id="473b9-139">9</span><span class="sxs-lookup"><span data-stu-id="473b9-139">9</span></span>|<span data-ttu-id="473b9-140">Gerenciamento de colegas Windows 10 acionado por piloto automático ou a diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="473b9-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



