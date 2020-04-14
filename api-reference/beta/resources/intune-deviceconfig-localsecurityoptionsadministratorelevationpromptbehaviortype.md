---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d0d5c8cd8a38589cef548d03c290015bd4368e12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439859"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="4607a-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="4607a-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

<span data-ttu-id="4607a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4607a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4607a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4607a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4607a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4607a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4607a-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="4607a-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="4607a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4607a-108">Members</span></span>
|<span data-ttu-id="4607a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4607a-109">Member</span></span>|<span data-ttu-id="4607a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4607a-110">Value</span></span>|<span data-ttu-id="4607a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4607a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4607a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4607a-112">notConfigured</span></span>|<span data-ttu-id="4607a-113">,0</span><span class="sxs-lookup"><span data-stu-id="4607a-113">0</span></span>|<span data-ttu-id="4607a-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="4607a-114">Not Configured</span></span>|
|<span data-ttu-id="4607a-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="4607a-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="4607a-116">1</span><span class="sxs-lookup"><span data-stu-id="4607a-116">1</span></span>|<span data-ttu-id="4607a-117">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="4607a-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="4607a-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4607a-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="4607a-119">duas</span><span class="sxs-lookup"><span data-stu-id="4607a-119">2</span></span>|<span data-ttu-id="4607a-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="4607a-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="4607a-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4607a-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="4607a-122">3D</span><span class="sxs-lookup"><span data-stu-id="4607a-122">3</span></span>|<span data-ttu-id="4607a-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="4607a-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="4607a-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="4607a-124">promptForCredentials</span></span>|<span data-ttu-id="4607a-125">4 </span><span class="sxs-lookup"><span data-stu-id="4607a-125">4</span></span>|<span data-ttu-id="4607a-126">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="4607a-126">Prompt for credentials</span></span>|
|<span data-ttu-id="4607a-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="4607a-127">promptForConsent</span></span>|<span data-ttu-id="4607a-128">5 </span><span class="sxs-lookup"><span data-stu-id="4607a-128">5</span></span>|<span data-ttu-id="4607a-129">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="4607a-129">Prompt for consent</span></span>|
|<span data-ttu-id="4607a-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="4607a-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="4607a-131">6 </span><span class="sxs-lookup"><span data-stu-id="4607a-131">6</span></span>|<span data-ttu-id="4607a-132">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="4607a-132">Prompt for consent for non-Windows binaries</span></span>|



