---
title: tipo de enumeração deviceManagementTemplateSubtype
description: Subtipo de modelo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4ed25a4700e28c3b1824b4b76d760343ced48774
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734200"
---
# <a name="devicemanagementtemplatesubtype-enum-type"></a><span data-ttu-id="31b69-103">tipo de enumeração deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="31b69-103">deviceManagementTemplateSubtype enum type</span></span>

<span data-ttu-id="31b69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31b69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31b69-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31b69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31b69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31b69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31b69-107">Subtipo de modelo</span><span class="sxs-lookup"><span data-stu-id="31b69-107">Template subtype</span></span>

## <a name="members"></a><span data-ttu-id="31b69-108">Membros</span><span class="sxs-lookup"><span data-stu-id="31b69-108">Members</span></span>
|<span data-ttu-id="31b69-109">Membro</span><span class="sxs-lookup"><span data-stu-id="31b69-109">Member</span></span>|<span data-ttu-id="31b69-110">Valor</span><span class="sxs-lookup"><span data-stu-id="31b69-110">Value</span></span>|<span data-ttu-id="31b69-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="31b69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31b69-112">none</span><span class="sxs-lookup"><span data-stu-id="31b69-112">none</span></span>|<span data-ttu-id="31b69-113">,0</span><span class="sxs-lookup"><span data-stu-id="31b69-113">0</span></span>|<span data-ttu-id="31b69-114">O modelo não tem subtipo</span><span class="sxs-lookup"><span data-stu-id="31b69-114">Template has no subtype</span></span>|
|<span data-ttu-id="31b69-115">Firewall</span><span class="sxs-lookup"><span data-stu-id="31b69-115">firewall</span></span>|<span data-ttu-id="31b69-116">1</span><span class="sxs-lookup"><span data-stu-id="31b69-116">1</span></span>|<span data-ttu-id="31b69-117">Subtipo de firewall de segurança do Endpoint</span><span class="sxs-lookup"><span data-stu-id="31b69-117">Endpoint security firewall subtype</span></span>|
|<span data-ttu-id="31b69-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="31b69-118">diskEncryption</span></span>|<span data-ttu-id="31b69-119">duas</span><span class="sxs-lookup"><span data-stu-id="31b69-119">2</span></span>|<span data-ttu-id="31b69-120">Subtipo de criptografia de disco do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="31b69-120">Endpoint security disk encryption subtype</span></span>|
|<span data-ttu-id="31b69-121">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="31b69-121">attackSurfaceReduction</span></span>|<span data-ttu-id="31b69-122">3D</span><span class="sxs-lookup"><span data-stu-id="31b69-122">3</span></span>|<span data-ttu-id="31b69-123">Subtipo de redução da superfície de ataque de segurança de pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="31b69-123">Endpoint security attack surface reduction subtype</span></span>|
|<span data-ttu-id="31b69-124">endpointDetectionReponse</span><span class="sxs-lookup"><span data-stu-id="31b69-124">endpointDetectionReponse</span></span>|<span data-ttu-id="31b69-125">4 </span><span class="sxs-lookup"><span data-stu-id="31b69-125">4</span></span>|<span data-ttu-id="31b69-126">Detecção de ponto de extremidade de segurança e subtipo de resposta do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="31b69-126">Endpoint security endpoint detection and response subtype</span></span>|
|<span data-ttu-id="31b69-127">accountProtection</span><span class="sxs-lookup"><span data-stu-id="31b69-127">accountProtection</span></span>|<span data-ttu-id="31b69-128">5 </span><span class="sxs-lookup"><span data-stu-id="31b69-128">5</span></span>|<span data-ttu-id="31b69-129">Subtipo de proteção da conta do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="31b69-129">Endpoint security account protection subtype</span></span>|
|<span data-ttu-id="31b69-130">vírus</span><span class="sxs-lookup"><span data-stu-id="31b69-130">antivirus</span></span>|<span data-ttu-id="31b69-131">6 </span><span class="sxs-lookup"><span data-stu-id="31b69-131">6</span></span>|<span data-ttu-id="31b69-132">Subtipo Anitivirus de segurança de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="31b69-132">Endpoint security anitivirus subtype</span></span>|





