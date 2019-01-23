---
title: tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType
description: Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413756"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="887fa-103">tipo de enum localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="887fa-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="887fa-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="887fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="887fa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="887fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="887fa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="887fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="887fa-107">Valores possíveis para LocalSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="887fa-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="887fa-108">Membros</span><span class="sxs-lookup"><span data-stu-id="887fa-108">Members</span></span>
|<span data-ttu-id="887fa-109">Membro</span><span class="sxs-lookup"><span data-stu-id="887fa-109">Member</span></span>|<span data-ttu-id="887fa-110">Valor</span><span class="sxs-lookup"><span data-stu-id="887fa-110">Value</span></span>|<span data-ttu-id="887fa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="887fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="887fa-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="887fa-112">notConfigured</span></span>|<span data-ttu-id="887fa-113">0</span><span class="sxs-lookup"><span data-stu-id="887fa-113">0</span></span>|<span data-ttu-id="887fa-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="887fa-114">Not Configured</span></span>|
|<span data-ttu-id="887fa-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="887fa-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="887fa-116">1</span><span class="sxs-lookup"><span data-stu-id="887fa-116">1</span></span>|<span data-ttu-id="887fa-117">Eleve sem aviso.</span><span class="sxs-lookup"><span data-stu-id="887fa-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="887fa-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="887fa-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="887fa-119">2</span><span class="sxs-lookup"><span data-stu-id="887fa-119">2</span></span>|<span data-ttu-id="887fa-120">Solicitar credenciais na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="887fa-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="887fa-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="887fa-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="887fa-122">3</span><span class="sxs-lookup"><span data-stu-id="887fa-122">3</span></span>|<span data-ttu-id="887fa-123">Solicitar consentimento na área de trabalho segura</span><span class="sxs-lookup"><span data-stu-id="887fa-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="887fa-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="887fa-124">promptForCredentials</span></span>|<span data-ttu-id="887fa-125">4</span><span class="sxs-lookup"><span data-stu-id="887fa-125">4</span></span>|<span data-ttu-id="887fa-126">Solicitação de credenciais</span><span class="sxs-lookup"><span data-stu-id="887fa-126">Prompt for credentials</span></span>|
|<span data-ttu-id="887fa-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="887fa-127">promptForConsent</span></span>|<span data-ttu-id="887fa-128">5</span><span class="sxs-lookup"><span data-stu-id="887fa-128">5</span></span>|<span data-ttu-id="887fa-129">Pedir consentimento</span><span class="sxs-lookup"><span data-stu-id="887fa-129">Prompt for consent</span></span>|
|<span data-ttu-id="887fa-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="887fa-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="887fa-131">6</span><span class="sxs-lookup"><span data-stu-id="887fa-131">6</span></span>|<span data-ttu-id="887fa-132">Solicitar consentimento para binários não-Windows</span><span class="sxs-lookup"><span data-stu-id="887fa-132">Prompt for consent for non-Windows binaries</span></span>|




