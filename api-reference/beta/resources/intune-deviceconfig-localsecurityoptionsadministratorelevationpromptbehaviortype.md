---
title: tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460524"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="86c48-103">tipo de enumeração localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="86c48-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="86c48-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86c48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86c48-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86c48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c48-106">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="86c48-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="86c48-107">Membros</span><span class="sxs-lookup"><span data-stu-id="86c48-107">Members</span></span>
|<span data-ttu-id="86c48-108">Membro</span><span class="sxs-lookup"><span data-stu-id="86c48-108">Member</span></span>|<span data-ttu-id="86c48-109">Valor</span><span class="sxs-lookup"><span data-stu-id="86c48-109">Value</span></span>|<span data-ttu-id="86c48-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="86c48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c48-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="86c48-111">notConfigured</span></span>|<span data-ttu-id="86c48-112">,0</span><span class="sxs-lookup"><span data-stu-id="86c48-112">0</span></span>|<span data-ttu-id="86c48-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="86c48-113">Not Configured</span></span>|
|<span data-ttu-id="86c48-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="86c48-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="86c48-115">1</span><span class="sxs-lookup"><span data-stu-id="86c48-115">1</span></span>|<span data-ttu-id="86c48-116">Elevar sem avisar.</span><span class="sxs-lookup"><span data-stu-id="86c48-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="86c48-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="86c48-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="86c48-118">duas</span><span class="sxs-lookup"><span data-stu-id="86c48-118">2</span></span>|<span data-ttu-id="86c48-119">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="86c48-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="86c48-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="86c48-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="86c48-121">3D</span><span class="sxs-lookup"><span data-stu-id="86c48-121">3</span></span>|<span data-ttu-id="86c48-122">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="86c48-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="86c48-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="86c48-123">promptForCredentials</span></span>|<span data-ttu-id="86c48-124">quatro</span><span class="sxs-lookup"><span data-stu-id="86c48-124">4</span></span>|<span data-ttu-id="86c48-125">Solicitar credenciais</span><span class="sxs-lookup"><span data-stu-id="86c48-125">Prompt for credentials</span></span>|
|<span data-ttu-id="86c48-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="86c48-126">promptForConsent</span></span>|<span data-ttu-id="86c48-127">0,5</span><span class="sxs-lookup"><span data-stu-id="86c48-127">5</span></span>|<span data-ttu-id="86c48-128">Solicitar consentimento</span><span class="sxs-lookup"><span data-stu-id="86c48-128">Prompt for consent</span></span>|
|<span data-ttu-id="86c48-129">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="86c48-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="86c48-130">6</span><span class="sxs-lookup"><span data-stu-id="86c48-130">6</span></span>|<span data-ttu-id="86c48-131">Solicitar consentimento para binários não Windows</span><span class="sxs-lookup"><span data-stu-id="86c48-131">Prompt for consent for non-Windows binaries</span></span>|





