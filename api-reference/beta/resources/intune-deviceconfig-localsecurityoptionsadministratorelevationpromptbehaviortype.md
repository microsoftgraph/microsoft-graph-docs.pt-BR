---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9dafe326466e18d8510e7494b37e91f5d0e2cff5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269011"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="69829-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="69829-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="69829-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69829-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69829-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69829-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69829-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69829-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69829-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="69829-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="69829-108">Membros</span><span class="sxs-lookup"><span data-stu-id="69829-108">Members</span></span>
|<span data-ttu-id="69829-109">Membro</span><span class="sxs-lookup"><span data-stu-id="69829-109">Member</span></span>|<span data-ttu-id="69829-110">Valor</span><span class="sxs-lookup"><span data-stu-id="69829-110">Value</span></span>|<span data-ttu-id="69829-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69829-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69829-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="69829-112">notConfigured</span></span>|<span data-ttu-id="69829-113">,0</span><span class="sxs-lookup"><span data-stu-id="69829-113">0</span></span>|<span data-ttu-id="69829-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="69829-114">Not Configured</span></span>|
|<span data-ttu-id="69829-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="69829-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="69829-116">1</span><span class="sxs-lookup"><span data-stu-id="69829-116">1</span></span>|<span data-ttu-id="69829-117">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="69829-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="69829-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="69829-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="69829-119">duas</span><span class="sxs-lookup"><span data-stu-id="69829-119">2</span></span>|<span data-ttu-id="69829-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="69829-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="69829-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="69829-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="69829-122">3D</span><span class="sxs-lookup"><span data-stu-id="69829-122">3</span></span>|<span data-ttu-id="69829-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="69829-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="69829-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="69829-124">promptForCredentials</span></span>|<span data-ttu-id="69829-125">4 </span><span class="sxs-lookup"><span data-stu-id="69829-125">4</span></span>|<span data-ttu-id="69829-126">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="69829-126">Prompt for credentials</span></span>|
|<span data-ttu-id="69829-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="69829-127">promptForConsent</span></span>|<span data-ttu-id="69829-128">5 </span><span class="sxs-lookup"><span data-stu-id="69829-128">5</span></span>|<span data-ttu-id="69829-129">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="69829-129">Prompt for consent</span></span>|
|<span data-ttu-id="69829-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="69829-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="69829-131">6 </span><span class="sxs-lookup"><span data-stu-id="69829-131">6</span></span>|<span data-ttu-id="69829-132">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="69829-132">Prompt for consent for non-Windows binaries</span></span>|




