---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a8d3be3ee9bd64f610820fb2e2eaa3b1352d272d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026688"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="c420f-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="c420f-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="c420f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c420f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c420f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c420f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c420f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c420f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c420f-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="c420f-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="c420f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c420f-108">Members</span></span>
|<span data-ttu-id="c420f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c420f-109">Member</span></span>|<span data-ttu-id="c420f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c420f-110">Value</span></span>|<span data-ttu-id="c420f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c420f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c420f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c420f-112">notConfigured</span></span>|<span data-ttu-id="c420f-113">,0</span><span class="sxs-lookup"><span data-stu-id="c420f-113">0</span></span>|<span data-ttu-id="c420f-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="c420f-114">Not Configured</span></span>|
|<span data-ttu-id="c420f-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="c420f-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="c420f-116">1 </span><span class="sxs-lookup"><span data-stu-id="c420f-116">1</span></span>|<span data-ttu-id="c420f-117">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="c420f-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="c420f-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="c420f-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="c420f-119">2 </span><span class="sxs-lookup"><span data-stu-id="c420f-119">2</span></span>|<span data-ttu-id="c420f-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="c420f-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="c420f-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="c420f-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="c420f-122">3 </span><span class="sxs-lookup"><span data-stu-id="c420f-122">3</span></span>|<span data-ttu-id="c420f-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="c420f-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="c420f-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="c420f-124">promptForCredentials</span></span>|<span data-ttu-id="c420f-125">4 </span><span class="sxs-lookup"><span data-stu-id="c420f-125">4</span></span>|<span data-ttu-id="c420f-126">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="c420f-126">Prompt for credentials</span></span>|
|<span data-ttu-id="c420f-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="c420f-127">promptForConsent</span></span>|<span data-ttu-id="c420f-128">5 </span><span class="sxs-lookup"><span data-stu-id="c420f-128">5</span></span>|<span data-ttu-id="c420f-129">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="c420f-129">Prompt for consent</span></span>|
|<span data-ttu-id="c420f-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="c420f-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="c420f-131">6 </span><span class="sxs-lookup"><span data-stu-id="c420f-131">6</span></span>|<span data-ttu-id="c420f-132">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="c420f-132">Prompt for consent for non-Windows binaries</span></span>|






