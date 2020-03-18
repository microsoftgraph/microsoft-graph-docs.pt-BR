---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03131e10101cfd582e558b68fc382b075602a069
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790367"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="6ac32-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6ac32-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="6ac32-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ac32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ac32-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ac32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ac32-106">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="6ac32-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="6ac32-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6ac32-107">Members</span></span>
|<span data-ttu-id="6ac32-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6ac32-108">Member</span></span>|<span data-ttu-id="6ac32-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6ac32-109">Value</span></span>|<span data-ttu-id="6ac32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ac32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ac32-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6ac32-111">notConfigured</span></span>|<span data-ttu-id="6ac32-112">,0</span><span class="sxs-lookup"><span data-stu-id="6ac32-112">0</span></span>|<span data-ttu-id="6ac32-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="6ac32-113">Not Configured</span></span>|
|<span data-ttu-id="6ac32-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="6ac32-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="6ac32-115">1</span><span class="sxs-lookup"><span data-stu-id="6ac32-115">1</span></span>|<span data-ttu-id="6ac32-116">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="6ac32-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="6ac32-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="6ac32-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="6ac32-118">duas</span><span class="sxs-lookup"><span data-stu-id="6ac32-118">2</span></span>|<span data-ttu-id="6ac32-119">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="6ac32-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="6ac32-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="6ac32-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="6ac32-121">3D</span><span class="sxs-lookup"><span data-stu-id="6ac32-121">3</span></span>|<span data-ttu-id="6ac32-122">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="6ac32-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="6ac32-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="6ac32-123">promptForCredentials</span></span>|<span data-ttu-id="6ac32-124">4 </span><span class="sxs-lookup"><span data-stu-id="6ac32-124">4</span></span>|<span data-ttu-id="6ac32-125">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="6ac32-125">Prompt for credentials</span></span>|
|<span data-ttu-id="6ac32-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="6ac32-126">promptForConsent</span></span>|<span data-ttu-id="6ac32-127">5 </span><span class="sxs-lookup"><span data-stu-id="6ac32-127">5</span></span>|<span data-ttu-id="6ac32-128">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="6ac32-128">Prompt for consent</span></span>|
|<span data-ttu-id="6ac32-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="6ac32-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="6ac32-130">6 </span><span class="sxs-lookup"><span data-stu-id="6ac32-130">6</span></span>|<span data-ttu-id="6ac32-131">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="6ac32-131">Prompt for consent for non-Windows binaries</span></span>|



