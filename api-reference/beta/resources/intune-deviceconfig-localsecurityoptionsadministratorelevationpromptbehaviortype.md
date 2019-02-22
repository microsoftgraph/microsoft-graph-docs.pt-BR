---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5deaccdd8e1f3707617fe2df06a5fec087a47625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139337"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="e4d0d-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="e4d0d-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="e4d0d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4d0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4d0d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4d0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4d0d-106">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="e4d0d-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="e4d0d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e4d0d-107">Members</span></span>
|<span data-ttu-id="e4d0d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e4d0d-108">Member</span></span>|<span data-ttu-id="e4d0d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e4d0d-109">Value</span></span>|<span data-ttu-id="e4d0d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4d0d-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e4d0d-111">notConfigured</span></span>|<span data-ttu-id="e4d0d-112">,0</span><span class="sxs-lookup"><span data-stu-id="e4d0d-112">0</span></span>|<span data-ttu-id="e4d0d-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="e4d0d-113">Not Configured</span></span>|
|<span data-ttu-id="e4d0d-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="e4d0d-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="e4d0d-115">1</span><span class="sxs-lookup"><span data-stu-id="e4d0d-115">1</span></span>|<span data-ttu-id="e4d0d-116">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="e4d0d-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="e4d0d-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e4d0d-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="e4d0d-118">duas</span><span class="sxs-lookup"><span data-stu-id="e4d0d-118">2</span></span>|<span data-ttu-id="e4d0d-119">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="e4d0d-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="e4d0d-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e4d0d-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="e4d0d-121">3D</span><span class="sxs-lookup"><span data-stu-id="e4d0d-121">3</span></span>|<span data-ttu-id="e4d0d-122">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="e4d0d-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="e4d0d-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="e4d0d-123">promptForCredentials</span></span>|<span data-ttu-id="e4d0d-124">quatro</span><span class="sxs-lookup"><span data-stu-id="e4d0d-124">4</span></span>|<span data-ttu-id="e4d0d-125">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="e4d0d-125">Prompt for credentials</span></span>|
|<span data-ttu-id="e4d0d-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="e4d0d-126">promptForConsent</span></span>|<span data-ttu-id="e4d0d-127">0,5</span><span class="sxs-lookup"><span data-stu-id="e4d0d-127">5</span></span>|<span data-ttu-id="e4d0d-128">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="e4d0d-128">Prompt for consent</span></span>|
|<span data-ttu-id="e4d0d-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="e4d0d-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="e4d0d-130">6</span><span class="sxs-lookup"><span data-stu-id="e4d0d-130">6</span></span>|<span data-ttu-id="e4d0d-131">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="e4d0d-131">Prompt for consent for non-Windows binaries</span></span>|




