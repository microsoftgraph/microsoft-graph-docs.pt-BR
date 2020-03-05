---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01f4cd1450e98b5c54e90d73af2e9d3278f24447
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529756"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="0ef97-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="0ef97-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="0ef97-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ef97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ef97-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ef97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ef97-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ef97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ef97-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="0ef97-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="0ef97-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0ef97-108">Members</span></span>
|<span data-ttu-id="0ef97-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0ef97-109">Member</span></span>|<span data-ttu-id="0ef97-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0ef97-110">Value</span></span>|<span data-ttu-id="0ef97-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ef97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef97-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0ef97-112">notConfigured</span></span>|<span data-ttu-id="0ef97-113">,0</span><span class="sxs-lookup"><span data-stu-id="0ef97-113">0</span></span>|<span data-ttu-id="0ef97-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="0ef97-114">Not Configured</span></span>|
|<span data-ttu-id="0ef97-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="0ef97-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="0ef97-116">1 </span><span class="sxs-lookup"><span data-stu-id="0ef97-116">1</span></span>|<span data-ttu-id="0ef97-117">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="0ef97-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="0ef97-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="0ef97-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="0ef97-119">2 </span><span class="sxs-lookup"><span data-stu-id="0ef97-119">2</span></span>|<span data-ttu-id="0ef97-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="0ef97-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="0ef97-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="0ef97-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="0ef97-122">3 </span><span class="sxs-lookup"><span data-stu-id="0ef97-122">3</span></span>|<span data-ttu-id="0ef97-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="0ef97-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="0ef97-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="0ef97-124">promptForCredentials</span></span>|<span data-ttu-id="0ef97-125">4 </span><span class="sxs-lookup"><span data-stu-id="0ef97-125">4</span></span>|<span data-ttu-id="0ef97-126">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="0ef97-126">Prompt for credentials</span></span>|
|<span data-ttu-id="0ef97-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="0ef97-127">promptForConsent</span></span>|<span data-ttu-id="0ef97-128">5 </span><span class="sxs-lookup"><span data-stu-id="0ef97-128">5</span></span>|<span data-ttu-id="0ef97-129">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="0ef97-129">Prompt for consent</span></span>|
|<span data-ttu-id="0ef97-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="0ef97-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="0ef97-131">6 </span><span class="sxs-lookup"><span data-stu-id="0ef97-131">6</span></span>|<span data-ttu-id="0ef97-132">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="0ef97-132">Prompt for consent for non-Windows binaries</span></span>|



