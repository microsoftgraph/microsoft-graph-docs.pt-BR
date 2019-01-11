---
title: tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 424c1193015d688019892d66ed07588358dcb8c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870879"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="3d1c6-103">tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="3d1c6-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="3d1c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d1c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d1c6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d1c6-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="3d1c6-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="3d1c6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3d1c6-108">Members</span></span>
|<span data-ttu-id="3d1c6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3d1c6-109">Member</span></span>|<span data-ttu-id="3d1c6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3d1c6-110">Value</span></span>|<span data-ttu-id="3d1c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d1c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d1c6-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="3d1c6-112">notConfigured</span></span>|<span data-ttu-id="3d1c6-113">0</span><span class="sxs-lookup"><span data-stu-id="3d1c6-113">0</span></span>|<span data-ttu-id="3d1c6-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="3d1c6-114">Not Configured</span></span>|
|<span data-ttu-id="3d1c6-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="3d1c6-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="3d1c6-116">1</span><span class="sxs-lookup"><span data-stu-id="3d1c6-116">1</span></span>|<span data-ttu-id="3d1c6-117">Eleve sem aviso.</span><span class="sxs-lookup"><span data-stu-id="3d1c6-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="3d1c6-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="3d1c6-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="3d1c6-119">2</span><span class="sxs-lookup"><span data-stu-id="3d1c6-119">2</span></span>|<span data-ttu-id="3d1c6-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="3d1c6-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="3d1c6-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="3d1c6-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="3d1c6-122">3</span><span class="sxs-lookup"><span data-stu-id="3d1c6-122">3</span></span>|<span data-ttu-id="3d1c6-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="3d1c6-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="3d1c6-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="3d1c6-124">promptForCredentials</span></span>|<span data-ttu-id="3d1c6-125">4</span><span class="sxs-lookup"><span data-stu-id="3d1c6-125">4</span></span>|<span data-ttu-id="3d1c6-126">Solicitação de credenciais</span><span class="sxs-lookup"><span data-stu-id="3d1c6-126">Prompt for credentials</span></span>|
|<span data-ttu-id="3d1c6-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="3d1c6-127">promptForConsent</span></span>|<span data-ttu-id="3d1c6-128">5</span><span class="sxs-lookup"><span data-stu-id="3d1c6-128">5</span></span>|<span data-ttu-id="3d1c6-129">Pedir consentimento</span><span class="sxs-lookup"><span data-stu-id="3d1c6-129">Prompt for consent</span></span>|
|<span data-ttu-id="3d1c6-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="3d1c6-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="3d1c6-131">6</span><span class="sxs-lookup"><span data-stu-id="3d1c6-131">6</span></span>|<span data-ttu-id="3d1c6-132">Solicitar consentimento para binários não-Windows</span><span class="sxs-lookup"><span data-stu-id="3d1c6-132">Prompt for consent for non-Windows binaries</span></span>|





