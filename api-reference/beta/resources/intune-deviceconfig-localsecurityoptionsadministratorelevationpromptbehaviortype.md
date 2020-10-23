---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ac5e864cdc35b7c39f64d10a369768406ae36546
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705670"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="73b4b-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="73b4b-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="73b4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73b4b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73b4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73b4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73b4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b4b-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="73b4b-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="73b4b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="73b4b-108">Members</span></span>
|<span data-ttu-id="73b4b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="73b4b-109">Member</span></span>|<span data-ttu-id="73b4b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="73b4b-110">Value</span></span>|<span data-ttu-id="73b4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="73b4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b4b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="73b4b-112">notConfigured</span></span>|<span data-ttu-id="73b4b-113">,0</span><span class="sxs-lookup"><span data-stu-id="73b4b-113">0</span></span>|<span data-ttu-id="73b4b-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="73b4b-114">Not Configured</span></span>|
|<span data-ttu-id="73b4b-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="73b4b-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="73b4b-116">1</span><span class="sxs-lookup"><span data-stu-id="73b4b-116">1</span></span>|<span data-ttu-id="73b4b-117">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="73b4b-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="73b4b-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="73b4b-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="73b4b-119">duas</span><span class="sxs-lookup"><span data-stu-id="73b4b-119">2</span></span>|<span data-ttu-id="73b4b-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="73b4b-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="73b4b-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="73b4b-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="73b4b-122">3D</span><span class="sxs-lookup"><span data-stu-id="73b4b-122">3</span></span>|<span data-ttu-id="73b4b-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="73b4b-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="73b4b-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="73b4b-124">promptForCredentials</span></span>|<span data-ttu-id="73b4b-125">4 </span><span class="sxs-lookup"><span data-stu-id="73b4b-125">4</span></span>|<span data-ttu-id="73b4b-126">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="73b4b-126">Prompt for credentials</span></span>|
|<span data-ttu-id="73b4b-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="73b4b-127">promptForConsent</span></span>|<span data-ttu-id="73b4b-128">5 </span><span class="sxs-lookup"><span data-stu-id="73b4b-128">5</span></span>|<span data-ttu-id="73b4b-129">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="73b4b-129">Prompt for consent</span></span>|
|<span data-ttu-id="73b4b-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="73b4b-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="73b4b-131">6 </span><span class="sxs-lookup"><span data-stu-id="73b4b-131">6</span></span>|<span data-ttu-id="73b4b-132">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="73b4b-132">Prompt for consent for non-Windows binaries</span></span>|





