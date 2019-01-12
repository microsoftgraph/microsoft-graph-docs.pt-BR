---
title: tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916821"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="b5de9-103">tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b5de9-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="b5de9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b5de9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5de9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b5de9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5de9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b5de9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5de9-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b5de9-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="b5de9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b5de9-108">Members</span></span>
|<span data-ttu-id="b5de9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b5de9-109">Member</span></span>|<span data-ttu-id="b5de9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b5de9-110">Value</span></span>|<span data-ttu-id="b5de9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5de9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5de9-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="b5de9-112">notConfigured</span></span>|<span data-ttu-id="b5de9-113">0</span><span class="sxs-lookup"><span data-stu-id="b5de9-113">0</span></span>|<span data-ttu-id="b5de9-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="b5de9-114">Not Configured</span></span>|
|<span data-ttu-id="b5de9-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="b5de9-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="b5de9-116">1</span><span class="sxs-lookup"><span data-stu-id="b5de9-116">1</span></span>|<span data-ttu-id="b5de9-117">Eleve sem aviso.</span><span class="sxs-lookup"><span data-stu-id="b5de9-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="b5de9-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="b5de9-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="b5de9-119">2</span><span class="sxs-lookup"><span data-stu-id="b5de9-119">2</span></span>|<span data-ttu-id="b5de9-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="b5de9-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="b5de9-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="b5de9-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="b5de9-122">3</span><span class="sxs-lookup"><span data-stu-id="b5de9-122">3</span></span>|<span data-ttu-id="b5de9-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="b5de9-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="b5de9-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="b5de9-124">promptForCredentials</span></span>|<span data-ttu-id="b5de9-125">4</span><span class="sxs-lookup"><span data-stu-id="b5de9-125">4</span></span>|<span data-ttu-id="b5de9-126">Solicitação de credenciais</span><span class="sxs-lookup"><span data-stu-id="b5de9-126">Prompt for credentials</span></span>|
|<span data-ttu-id="b5de9-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="b5de9-127">promptForConsent</span></span>|<span data-ttu-id="b5de9-128">5</span><span class="sxs-lookup"><span data-stu-id="b5de9-128">5</span></span>|<span data-ttu-id="b5de9-129">Pedir consentimento</span><span class="sxs-lookup"><span data-stu-id="b5de9-129">Prompt for consent</span></span>|
|<span data-ttu-id="b5de9-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="b5de9-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="b5de9-131">6</span><span class="sxs-lookup"><span data-stu-id="b5de9-131">6</span></span>|<span data-ttu-id="b5de9-132">Solicitar consentimento para binários não-Windows</span><span class="sxs-lookup"><span data-stu-id="b5de9-132">Prompt for consent for non-Windows binaries</span></span>|





